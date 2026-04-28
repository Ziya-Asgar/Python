# Strings

- [Strings](#strings)
  - [Creating strings](#creating-strings)
  - [Accessing strings](#accessing-strings)
  - [F-strings](#f-strings)
  - [`str.upper()` and `str.lower()`](#strupper-and-strlower)
  - [Searching in a string](#searching-in-a-string)
    - [`in` operator](#in-operator)
    - [The `find` method](#the-find-method)
    - [The `index` method](#the-index-method)
  - [Removing unwanted characters from the beginning and end of a string](#removing-unwanted-characters-from-the-beginning-and-end-of-a-string)
  - [`startswith`](#startswith)
  - [`count`](#count)
  - [`replace`](#replace)
  - [`split`](#split)
  - [`join`](#join)
  - [`capitalize`](#capitalize)
  - [Escaping](#escaping)
  - [Raw strings](#raw-strings)

---

---

## Creating strings

You can write string literals using either single quotes `'` or double quotes `"` (double quotes are generally favored):

```py
a = 'one way of writing a string'
b = "another way"
```

For multiline strings with line breaks, you can use triple quotes, either `'''` or `"""`:

```py
c = """
This is a longer string that
spans multiple lines
"""
```

---

---

## Accessing strings

You can access the characters of a string with the bracket operator:

```py
fruit = "banana"

print(fruit[1]) # a
print(fruit[-2]) # n
print(fruit[0:4]) # bana
print(fruit[2:2]) # '' - returns an empty string
```

---

---

## F-strings

A formatted string literal (often referred to simply as an f-string) allows Python expressions to be used within string literals.

```py
variable = 1

print(f'{variable}') # 1
print(f'I have {variable} car') # I have 1 car
```

---

---

## `str.upper()` and `str.lower()`

The string method `upper` takes a string and returns a new string with all uppercase letters:

```py
text = "some text"

print(text.upper()) # SOME TEXT
```

The string method `lower` takes a string and returns a new string with all lowercase letters:

```py
text = "SOME TEXT"

print(text.lower()) # some text
```

---

---

## Searching in a string

### `in` operator

`in` is a boolean operator that takes two strings and returns `True` if the first appears as a substring in the second:

```py
text = "text"

print("x" in text)  # True
print("te" in text) # True
print("text" in text) # True
print("test" in text) # False
```

### The `find` method

There is a string method named `find` that searches for the position of one string within another:

```py
text = "text"

print(text.find('x')) # 2
print(text.find('te')) # 0
print(text.find('text')) # 0
print(text.find('test')) # -1
```

It can take the index as a second argument where it should start searching:

```py
text = "some text"

print(text.find('t', 2)) # 5
print(text.find('t', 6)) # 8
print(text.find('some', 1)) # -1
```

The `rfind` is similar to `find`. However, it returns the position of the first character of the last occurrence of substring in the string.

### The `index` method

The `index` method returns the position at the first occurrence of the specified value.

```py
text = "some text"

print(text.index("e")) # 3
print(text.index("text")) # 5
```

Note that the difference between `find` and `index` is that `index` raises an exception if the string isn’t found (versus returning `–1`).

---

---

## Removing unwanted characters from the beginning and end of a string

The `.strip()` method removes punctuation marks, specific symbols, or other unwanted characters from both ends of the string. By default, it removes white space (spaces, tabs, or newlines) from the beginning and end of a string:

```py
line = '  Here we go  '
print(line.strip())
#'Here we go'

line = '-Here-we-go-'
print(line.strip("-"))
# Here-we-go
```

The `rstrip` method strips the unwanted characters from the right side of a string:

```py
line = '  Here we go  '

print(line.rstrip())
#   Here we go
```

The `lstrip` method strips unwanted characters from the left side of a string:

```py
line = '  Here we go  '

print(line.lstrip())
# Here we go
```

---

---

## `startswith`

The `startswith` string method checks if a string starts with certain characters and returns `True` or `False`:

```py
text = "some text"

print(text.startswith("s")) # True
print(text.startswith("some")) # True
print(text.startswith("me")) # False
```

---

---

## `count`

The `count` method counts the provided characters in a string:

```py
text = "banana"

print(text.count("a")) # 3
print(text.count("an")) # 2
```

---

---

## `replace`

Although strings are immutable, we can still use the `replace` method to copy a string and change part of it:

```py
sentence1 = "This is a string."
sentence2 = sentence1.replace("string", "longer string")

print(sentence1) # This is a string.
print(sentence2) # This is a longer string.
```

---

---

## `split`

If you want to break a string into the list of words, you can use the `split` method:

```py
sentence = 'Here is a simple sentence.'
listVar = sentence.split()

print(listVar) # ['Here', 'is', 'a', 'simple', 'sentence.']

print(listVar[1]) # is
```

You can call `split` with an optional argument called a delimiter that specifies which characters to use as word boundaries. The following example uses a hyphen as a delimiter:

```py
shortStr = 'A-short-string'

delimiter = '-'
print(shortStr.split(delimiter)) # ['A', 'short', 'string']
```

---

---

## `join`

The `join` method takes a list of strings and concatenates the elements. `join` is a **string method**, so you have to invoke it on the delimiter and pass the list as a parameter:

```py
listVar = ['Here', 'is', 'a', 'simple', 'sentence.']
delimiter = ' '

print(delimiter.join(listVar)) # Here is a simple sentence.
print('-'.join(listVar)) # Here-is-a-simple-sentence.
```

---

---

## `capitalize`

The `capitalize` method capitalizes the string

```py
print("testing and testing".capitalize()) # Testing and testing
```

---

---

## Escaping

Some characters has special meanings in a string. For example, `\n` means new line:

```py
print('12\n34')
"""
12
34
"""
```

To escape the special meaning of certain characters in a string, we can use `\`:

```py
print('12\\n34') # 12\n34
```

---

---

## Raw strings

To avoid special meaning of certain characters, we can also add `r` before the leading quote of the string, which means that the characters should be interpreted as is. The `r` stands for raw:

```py
print(r"12\n34") # 12\n34
```

---

---
