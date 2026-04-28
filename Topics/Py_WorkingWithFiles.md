# Working with Files

- [Working with Files](#working-with-files)
  - [`open` function](#open-function)
  - [Using the `with` keyword](#using-the-with-keyword)
  - [`closed` property](#closed-property)
  - [Reading files with the `read` method](#reading-files-with-the-read-method)
  - [Reading files with the `readline` method](#reading-files-with-the-readline-method)
  - [Opening files in `"w"` mode and writing with the `write` method](#opening-files-in-w-mode-and-writing-with-the-write-method)
  - [Opening files in `"x"` mode](#opening-files-in-x-mode)
  - [Opening files in `"a"` mode](#opening-files-in-a-mode)
  - [Opening files in `"r+"` mode](#opening-files-in-r-mode)

---

---

## `open` function

To open a file using Python, we use the `open` function. If the open is successful, the operating system returns a file handle. The file handle is not the actual data contained in the file, but instead it is a “handle” that we can use to read the data. You are given a handle if the requested file exists and you have the proper permissions to read the file. We can use either a relative or absolute path with the `open` function:

```py
import os

file_path = os.path.join(os.getcwd(), "text.txt")

fhand = open(file_path, encoding="utf-8")
count = 0
for line in fhand:
  count = count + 1

fhand.close()

print('Line Count', count)
```

A few notes about opening a file:

- Normally, files are opened in the text mode, that means, you read and write strings from and to the file, which are encoded in a specific encoding. If encoding is not specified, the default is platform dependent. Because UTF-8 is the modern de-facto standard, providing `encoding="utf-8"` argument is recommended unless you know that you need to use a different encoding.

- By default, the file is opened in read-only mode `"r"`.

- We can then treat the file object like a list and iterate over the lines like so.

- When you use `open` to create file objects, it is recommended to close the file when you are finished with it. Closing the file releases its resources back to the operating system

---

---

## Using the `with` keyword

It is good practice to use the `with` keyword when dealing with file objects. The advantage is that the file is properly closed after the job is done, even if an exception is raised at some point.

```py
import os

file_path = os.path.join(os.getcwd(), "text.txt")

with open(file_path, encoding="utf-8") as fhand:
  for line in fhand:
    print(str.rstrip(line))
```

If you’re not using the `with` keyword, then you should call `close()` to close the file and immediately free up any system resources used by it.

---

---

## `closed` property

We can check that the file has been closed using the `closed` property on the file handle.

```py
import os

file_path = os.path.join(os.getcwd(), "text.txt")

with open(file_path, encoding="utf-8") as fhand:
  for line in fhand:
    print(str.rstrip(line))

print(fhand.closed) # True
```

---

---

## Reading files with the `read` method

In addition to reading files using the `for` loop, we can also read the file’s contents by calling the `read(<size>)` method. It reads some quantity of data and returns it as a string (in text mode) or bytes object (in binary mode). It accepts an optional numeric size argument. When the size is omitted or negative, the entire contents of the file will be read and returned. It is a good idea to store the output of `read` as a variable because each call to `read` exhausts the resource.

Example of `read` using `with`:

```py
import os

file_path = os.path.join(os.getcwd(), "text.txt")

with open(file_path, encoding="utf-8") as fhand:
  text = fhand.read()

print(len(text))
print(text[:20])
```

Example of `read` without `with`:

```py
import os

file_path = os.path.join(os.getcwd(), "text.txt")

fhand = open(file_path, encoding="utf-8")
text = fhand.read()

fhand.close()

print(len(text))
print(text[:20])
```

Here is an example of `read` with the `size` argument (using the `with` keyword):

```py
import os

file_path = os.path.join(os.getcwd(), "text.txt")

with open(file_path, encoding="utf-8") as fhand:
  text = fhand.read(20)

print(len(text)) # 20
print(text)
```

Here is an example of `read` with the `size` argument (without using the `with` keyword):

```py
import os

file_path = os.path.join(os.getcwd(), "text.txt")

fhand = open(file_path, encoding="utf-8")
text = fhand.read(20)

fhand.close()

print(len(text)) # 20
print(text)
```

If the end of the file has been reached, `read()` will return an empty string ('').

If the file is too large to fit in main memory, you might prefer to write your program to read the file in chunks using a `for` or `while` loop.

---

---

## Reading files with the `readline` method

`readline()` reads a single line from the file; a newline character (`\n`) is left at the end of the string, and is only omitted on the last line of the file if the file doesn’t end in a newline.

```py
import os

file_path = os.path.join(os.getcwd(), "text.txt")

with open(file_path, encoding="utf-8") as fhand:
  text = fhand.readline()

print(len(text))
print(text)
```

---

---

## Opening files in `"w"` mode and writing with the `write` method

To write a file, you have to open it with mode `“w”` as a second parameter. If the file doesn’t exist, a new one is created. If the file already exists, opening it in the write mode clears out the old data and starts fresh.

`open('text.txt', 'w')` just opens the file for writing. It doesn't do the actual writing. The `write` method of the file handle object puts data into the file, returning the number of characters written. The default write mode is text for writing (and reading) strings.

```py
import os

file_path = os.path.join(os.getcwd(), "text.txt")

with open(file_path, "w", encoding="utf-8") as fhand:
  fhand.write("This is the first line to be written.\n")
```

The file object keeps track of where it is, so if you call `write` again, it adds the new data to the end.

```py
import os

file_path = os.path.join(os.getcwd(), "text.txt")

with open(file_path, "w", encoding="utf-8") as fhand:
  fhand.write("This is the first line to be written.\n")
  fhand.write("This is the second line to be written.\n")
```

Remember if you are not using the `with` keyword, you have to close the file, when you are done writing, to make sure that the last bit of data is physically written to the disk so it will not be lost if the power goes off.

```py
import os

file_path = os.path.join(os.getcwd(), "text.txt")

fhand = open(file_path, "w", encoding="utf-8")

fhand.write("This is the first line to be written.\n")
fhand.write("This is the second line to be written.\n")

fhand.close()
```

> When we open files to read from them, Python makes sure that all open files are closed when the program ends. When we are writing files, we want to explicitly close the files so as to leave nothing to chance.

---

Other types of objects need to be converted – either to a string (in text mode) or a bytes object (in binary mode) – before writing them:

```py
import os

file_path = os.path.join(os.getcwd(), "text.txt")

tup = ("hello", 2, "you")

with open(file_path, "w", encoding="utf-8") as fhand:
  stringified = str(tup)
  fhand.write(stringified)
```

---

---

## Opening files in `"x"` mode

There is also the `"x"` file mode, which creates a writable file but fails if the file path already exists.

```py
import os

file_path = os.path.join(os.getcwd(), "text2.txt")

# this runs the first time when the file doesn't exist
# it throws an exception if run the second time, when the file exists
with open(file_path, "x", encoding="utf-8") as fhand:
  fhand.write("Here is some text.")

with open(file_path, encoding="utf-8") as fhand:
  print(fhand.read()) # Here is some text.
```

---

---

## Opening files in `"a"` mode

The `"a"` mode appends to the file. It creates the file if it does not already exist:

```py
import os

file_path = os.path.join(os.getcwd(), "text2.txt")

with open(file_path, "a", encoding="utf-8") as fhand:
  fhand.write("\nSome more data for the file.")

with open(file_path, encoding="utf-8") as fhand:
  print(fhand.read()) # Here is some text.
```

---

---

## Opening files in `"r+"` mode

The `"r+"` mode returns a file handle that could be used both to read from and write to the file:

```py
import os

file_path = os.path.join(os.getcwd(), "text.txt")

with open(file_path, "r+", encoding="utf-8") as fhand:
  fhand.write("This is to be written into the file.")
  print(fhand.read()) # This is to be written into the file.
```

---

In addition to the above modes, you can specify if the file should be handled as binary or text mode using the `"t"` and `"b"` flags. `"rt"` is the default value. So, if no mode is specified with the `open` function, these are going to be assumed.

---

---
