# Python

- [Python](#python)
  - [Some Useful Links](#some-useful-links)
  - [Intro](#intro)
  - [Modules](#modules)
  - [Creating and assigning to variables](#creating-and-assigning-to-variables)
  - [Strings](#strings)
    - [Creating strings](#creating-strings)
    - [Accessing strings](#accessing-strings)
    - [F-strings](#f-strings)
    - [`str.upper()` and `str.lower()`](#strupper-and-strlower)
    - [Searching in a string](#searching-in-a-string)
      - [`in` operator](#in-operator)
      - [The `find` method](#the-find-method)
      - [The `index` method](#the-index-method)
    - [Removing white space from the beginning and end of strings](#removing-white-space-from-the-beginning-and-end-of-strings)
    - [`startswith`](#startswith)
    - [`count`](#count)
    - [`replace`](#replace)
    - [`split`](#split)
    - [`join`](#join)
    - [`capitalize`](#capitalize)
    - [Escaping](#escaping)
    - [Raw strings](#raw-strings)
  - [Binary operations](#binary-operations)
  - [Asking the user for input](#asking-the-user-for-input)
  - [Type Conversion](#type-conversion)
  - [Conditionals](#conditionals)
    - [Comparison Operators](#comparison-operators)
    - [Logical Operators](#logical-operators)
    - [`if` statement](#if-statement)
  - [Error Handling](#error-handling)
    - [`raise`](#raise)
  - [Functions](#functions)
    - [Creating a Function](#creating-a-function)
      - [`return`](#return)
      - [Positional and Keyword arguments](#positional-and-keyword-arguments)
      - [Assigning variables outside of a function with `global`](#assigning-variables-outside-of-a-function-with-global)
    - [Lambda functions](#lambda-functions)
    - [`*args` and `**kwargs`](#args-and-kwargs)
    - [Decorators](#decorators)
    - [Some Built-in Functions](#some-built-in-functions)
      - [`max` and `min`](#max-and-min)
      - [`len`](#len)
      - [`sum`](#sum)
      - [`dir`](#dir)
      - [`help`](#help)
      - [`range`](#range)
      - [`enumerate`](#enumerate)
      - [`zip`](#zip)
      - [`reversed`](#reversed)
      - [`map`](#map)
      - [`filter`](#filter)
  - [Generators](#generators)
  - [Loops](#loops)
    - [`while` loop](#while-loop)
    - [`for` loop](#for-loop)
    - [`break` statement](#break-statement)
    - [`continue` statement](#continue-statement)
  - [`random` module](#random-module)
  - [`math` module](#math-module)
  - [`os` module](#os-module)
    - [`getcwd()`](#getcwd)
    - [`listdir()`](#listdir)
    - [`makedirs()`](#makedirs)
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
  - [Lists](#lists)
    - [Creating a list](#creating-a-list)
    - [Accessing list items](#accessing-list-items)
    - [Using the `in` operator with lists](#using-the-in-operator-with-lists)
    - [Looping through lists with the `for` loop](#looping-through-lists-with-the-for-loop)
    - [Using `+` and `*` operators with lists](#using--and--operators-with-lists)
    - [List Methods](#list-methods)
      - [`append`](#append)
      - [`extend`](#extend)
      - [`insert`](#insert)
      - [`sort`](#sort)
      - [The `sorted` function](#the-sorted-function)
      - [`reverse`](#reverse)
    - [Deleting List Elements](#deleting-list-elements)
  - [Dictionaries](#dictionaries)
    - [Creating a dictionary](#creating-a-dictionary)
    - [Accessing dictionary items](#accessing-dictionary-items)
    - [Adding dictionary items](#adding-dictionary-items)
    - [Using `len` function on dictionaries](#using-len-function-on-dictionaries)
    - [Using `in` operator with dictionaries](#using-in-operator-with-dictionaries)
    - [The `values` method](#the-values-method)
    - [The `keys` method](#the-keys-method)
    - [The `items` method](#the-items-method)
    - [`get`](#get)
    - [`update`](#update)
    - [Looping through dictionary items](#looping-through-dictionary-items)
    - [Deleting items from a dictionary](#deleting-items-from-a-dictionary)
    - [Dictionary unpacking with `**`](#dictionary-unpacking-with-)
  - [Tuples](#tuples)
    - [Creating a tuple](#creating-a-tuple)
    - [Accessing tuple elements](#accessing-tuple-elements)
    - [Some possible modifications in a tuple](#some-possible-modifications-in-a-tuple)
    - [Using `+` and `*` operators with tuples](#using--and--operators-with-tuples)
    - [`count`](#count-1)
  - [Iterable Unpacking](#iterable-unpacking)
  - [Classes](#classes)
    - [Creating a class and an object instance](#creating-a-class-and-an-object-instance)
    - [Accessing class members with `getattr`](#accessing-class-members-with-getattr)
    - [Name mangling and naming convention for private class members](#name-mangling-and-naming-convention-for-private-class-members)
    - [Class attributes vs instance attributes](#class-attributes-vs-instance-attributes)
    - [`__dict__` attribute](#__dict__-attribute)
  - [Sets](#sets)
    - [Creating sets](#creating-sets)
    - [Mathematical operations on sets](#mathematical-operations-on-sets)
      - [Union](#union)
      - [Intersection](#intersection)
      - [Difference](#difference)
      - [Symmetric difference](#symmetric-difference)
    - [`issubset`](#issubset)
    - [`issuperset`](#issuperset)
    - [`isdisjoint`](#isdisjoint)
    - [`add`](#add)
    - [`clear`](#clear)
    - [Deleting set elements](#deleting-set-elements)
    - [Equality of sets](#equality-of-sets)
  - [List, Set, and Dictionary Comprehensions](#list-set-and-dictionary-comprehensions)
  - [Regex](#regex)
    - [Using the `search` method from `re`](#using-the-search-method-from-re)
    - [Searching the beginning of the file using the `^`](#searching-the-beginning-of-the-file-using-the-)
    - [Searching the end of the file using the `$`](#searching-the-end-of-the-file-using-the-)
    - [Match any character once with `.`](#match-any-character-once-with-)
    - [Match any character zero or more times with `*`](#match-any-character-zero-or-more-times-with-)
    - [Match any character once or more times with `+`](#match-any-character-once-or-more-times-with-)
    - [Match any character once or zero time with `?`](#match-any-character-once-or-zero-time-with-)
    - [Note about greedy mode](#note-about-greedy-mode)
    - [Using the `findall` method from `re`](#using-the-findall-method-from-re)
    - [Using square brackets in Regex](#using-square-brackets-in-regex)
    - [Using parentheses in Regex](#using-parentheses-in-regex)
    - [Matching whitespace character with `\s` and non-whitespace character with `\S`](#matching-whitespace-character-with-s-and-non-whitespace-character-with-s)
    - [Word boundary with `\b`](#word-boundary-with-b)
    - [Non-word boundary with `\B`](#non-word-boundary-with-b)
    - [Match digits with `\d` and non-digits with `\D`](#match-digits-with-d-and-non-digits-with-d)
    - [Table of some regex methods](#table-of-some-regex-methods)
  - [Python Package index and pip](#python-package-index-and-pip)
  - [Network](#network)
  - [Date and Time](#date-and-time)
    - [`now`](#now)
    - [`timedelta`](#timedelta)
    - [Formatting `datetime` objects as strings](#formatting-datetime-objects-as-strings)
    - [Converting string dates to `datetime` objects](#converting-string-dates-to-datetime-objects)
    - [Locale-specific date formatting](#locale-specific-date-formatting)

<hr>
<hr>

## Some Useful Links

- https://www.py4e.com/lessons
- https://dabeaz-course.github.io/practical-python/Notes/00_Setup.html
- https://docs.python.org/3/
- https://wesmckinney.com/book/python-basics

<hr>
<hr>

## Intro

You can use Python by creating a file with `.py` extension and write the Python code in that file. If you want to run the python code in that file, you use `python fileName.py` in the terminal.

Or you can use the terminal to write the python code directly. On Windows machines, if you have the **py.exe** launcher installed, you can use the `py` or `python` command.

<hr>

To print something to the terminal using Python, we use the `print()` command:

```py
print("Hello World!")
```

IPython (http://ipython.org/) provides a programming environment that is optimized for interactive computing with Python. Once the individual steps are working, one can use the IPython command `%history` to get the commands used. One can use either copy/paste that history, or save it directly to a file with `%history -f [fname]`.

<hr>

## Modules

In Python, a module is simply a file with the `.py` extension containing Python code. Let's say we have a file named `module.py` with the below code:

```py
# module.py
simpleString = "simple string"

def func(arg):
  print(arg)
```

We can import and use the `module.py` in the `test.py`, located in the same directory, this way:

```py
# test.py
import module

print(module.simpleString) # simple string
module.func('running module.func from test.py') # running module.func from test.py
```

By using the `as` keyword, you can give imports different variable names:

```py
import module as md
# from module import simpleString, func

print(md.simpleString) # simple string
md.func('running module.func from test.py') # running module.func from test.py
```

We can also import specific variables:

```py
# test.py
from module import simpleString, func

print(simpleString) # simple string
func('running module.func from test.py') # running module.func from test.py
```

The command `from <module_name> import *` imports all variables and functions from `<module_name>` into the current workspace. However, use of this syntax is discouraged! It clutters up the current workspace, and one risks overwriting existing variables with the same name as an imported variable.

<hr>

## Creating and assigning to variables

An important characteristic of the Python language is the consistency of its object model. Every number, string, data structure, function, class, module, and so on exists in the Python interpreter in its own “box,” which is referred to as a Python object. Each object has an associated type (e.g., integer, string, or function) and internal data.

<hr>

There is no specific keyword to initiate a variable in Python. To create a variable, we just use a variable name:

```py
var = 1
anotherVar = "some text"

print(var) # 1
print(anotherVar) # some text
```

When assigning a variable (or name) in Python, you are creating a reference to the object shown on the right-hand side of the equality sign.

Assignment is also referred to as binding, as we are binding a name to an object. Variable names that have been assigned may occasionally be referred to as bound variables.

Suppose, we have the variable `a` and we assign it's value to the variable `b`:

```py
a = [1, 2, 3]
b = a
```

In some languages, the assignment of `b` will cause the data `[1, 2, 3]` to be copied. In Python, `a` and `b` actually now refer to the same object, the original list `[1, 2, 3]`:

```py
a = [1, 2, 3]
b = a

print(a) # [1, 2, 3]
print(b) # [1, 2, 3]

a.append(4)

print(a) # [1, 2, 3, 4]
print(b) # [1, 2, 3, 4]
```

<hr>

To check whether two variables refer to the same object, you can use the `is` operator.

```py
a = 'banana'
b = 'banana'

print(a is b) # True
```

Use `is not` to check that two objects are not the same:

```py
a = 'banana'

# the list function always creates a new Python list (i.e., a copy)
b = list('banana')

print(a is not b) # True
```

<hr>

We can assign the same value to multiple variables at once:

```py
var1 = var2 = var3 = "some variable"

print(var1) # some variable
print(var2) # some variable
print(var3) # some variable
```

<hr>

To learn the type of data, we can use the `type()` command:

```py
string = type("Hello World")
integer = type(1)
float_number = type(3.2)

print(string)
# <class 'str'>

print(integer)
# <class 'int'>

print(float_number)
# <class 'float'>
```

<hr>
<hr>

## Strings

A string is a sequence of characters.

<hr>

### Creating strings

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

<hr>

### Accessing strings

You can access the characters of a string with the bracket operator:

```py
fruit = "banana"

print(fruit[1]) # a
print(fruit[-2]) # n
print(fruit[0:4]) # bana
print(fruit[2:2]) # '' - returns an empty string
```

<hr>

### F-strings

A formatted string literal (often referred to simply as an f-string) allows Python expressions to be used within string literals.

```py
variable = 1

print(f'{variable}') # 1
print(f'I have {variable} car') # I have 1 car
```

<hr>

### `str.upper()` and `str.lower()`

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

<hr>

### Searching in a string

#### `in` operator

`in` is a boolean operator that takes two strings and returns `True` if the first appears as a substring in the second:

```py
text = "text"

print("x" in text)  # True
print("te" in text) # True
print("text" in text) # True
print("test" in text) # False
```

#### The `find` method

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

#### The `index` method

The `index` method returns the position at the first occurrence of the specified value.

```py
text = "some text"

print(text.index("e")) # 3
print(text.index("text")) # 5
```

Note that the difference between `find` and `index` is that `index` raises an exception if the string isn’t found (versus returning `–1`).

<hr>

### Removing white space from the beginning and end of strings

To remove white space (spaces, tabs, or newlines) from the beginning and end of a string, we can use the `strip` method:

```py
line = '  Here we go  '

print(line.strip())
#'Here we go'
```

The `rstrip` method strips white spaces from the right side of a string:

```py
line = '  Here we go  '

print(line.rstrip())
#   Here we go
```

The `lstrip` method strips white spaces from the left side of a string:

```py
line = '  Here we go  '

print(line.lstrip())
# Here we go
```

<hr>

### `startswith`

The `startswith` string method checks if a string starts with certain characters and returns `True` or `False`:

```py
text = "some text"

print(text.startswith("s")) # True
print(text.startswith("some")) # True
print(text.startswith("me")) # False
```

<hr>

### `count`

The `count` method counts the provided characters in a string:

```py
text = "banana"

print(text.count("a")) # 3
print(text.count("an")) # 2
```

<hr>

### `replace`

Although strings are immutable, we can still use the `replace` method to copy a string and change part of it:

```py
sentence1 = "This is a string."
sentence2 = sentence1.replace("string", "longer string")

print(sentence1) # This is a string.
print(sentence2) # This is a longer string.
```

<hr>

### `split`

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

<hr>

### `join`

The `join` method takes a list of strings and concatenates the elements. `join` is a **string method**, so you have to invoke it on the delimiter and pass the list as a parameter:

```py
listVar = ['Here', 'is', 'a', 'simple', 'sentence.']
delimiter = ' '

print(delimiter.join(listVar)) # Here is a simple sentence.
print('-'.join(listVar)) # Here-is-a-simple-sentence.
```

<hr>

### `capitalize`

The `capitalize` method capitalizes the string

```py
print("testing and testing".capitalize()) # Testing and testing
```

<hr>

### Escaping

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

<hr>

### Raw strings

To avoid special meaning of certain characters, we can also add `r` before the leading quote of the string, which means that the characters should be interpreted as is. The `r` stands for raw:

```py
print(r"12\n34") # 12\n34
```

<hr>
<hr>

## Binary operations

Most of the binary math operations and comparisons use familiar mathematical syntax in Python.

- Add a and b with `+`

```py
a = 1
b = 2

print(a + b) # 3
```

- Subtract b from a with `-`

```py
a = 1
b = 2

print(a - b) # -1
```

- Multiply a by b with `*`

```py
a = 1
b = 2

print(a * b) # 2
```

- Divide a by b with `/`

```py
a = 1
b = 2

print(a / b) # 0.5
```

- Floor-divide a by b with `//`, dropping any fractional remainder. Using this always returns an integer:

```py
a = 1
b = 2

print(a // b) # 0
```

- Raise a to the b power with `**`

```py
a = 5
b = 2

exponentiation = a ** b

print(exponentiation) # 25
```

The modulus operator works on integers and yields the remainder of the division. In Python, the modulus operator is a percent sign (`%`).

```py
remainder = 7 % 3

print(remainder) # 1
```

<hr>

`+` and `*` are an addition and a multiplication operators. But they are also used for string concatenation:

```py
strNum1 = '100'
strNum2 = '150'

print(strNum1 + strNum2) # 100150
```

```py
strNum1 = 'Test '
strNum2 = 3

print(strNum1 * strNum2) # Test Test Test
```

<hr>
<hr>

## Asking the user for input

Sometimes we would like to take the value for a variable from a user. Python provides a built-in function called `input` that gets input from the keyboard. When this function is called, the program stops and waits for the user to type something. When the user presses Return or Enter, the program resumes and `input` returns what the user typed as a string.

```py
inp = input()
# user types "testing"

print(inp)
# testing
```

You can pass a string to the `input` function to be displayed to the user while asking for an input:

```py
name = input("What is your name?\n")

print(f"Hello, {name}")
```

<hr>
<hr>

## Type Conversion

You can convert a value to integer using the `int()` function:

```py
string = type("1")
integer = type(int("1"))

print(string)
# <class 'str'>

print(integer)
# <class 'int'>
```

`float` converts integers and strings to floating-point numbers:

```py
print(float(32))
# 32.0
print(float('3.14159'))
# 3.14159
```

Many Python objects can be converted to a string using the `str` function:

```py
print(type(str(12)))
# <class 'str'>
```

<hr>
<hr>

## Conditionals

### Comparison Operators

Here is the list of **comparison operators** in Python:

- `x == y` - is x equal to y?
- `x != y` - is x not equal to y?
- `x > y` - is x greater than y?
- `x < y` - is x less than y?
- `x >= y` - is x greater than or equal to y?
- `x <= y` - is x less than or equal to y?
- `x is y` - is x the same as y?
- `x is not y` - is x not the same as y?

```py
print(5 == 5) # True
print(5 == 6) # False

print(5 != 5) # False
print(5 != 6) # True

print(5 > 5) # False
print(5 > 6) # False

print(5 < 5) # False
print(5 < 6) # True

print(5 >= 5) # True
print(5 >= 6) # False

print(5 <= 5) # True
print(5 <= 6) # True

# the operators "is" and "is not" are not used with numbers
five = 5
six = 6

print(five is five) # True
print(five is six) # False

print(five is not five) # False
print(five is not six) # True
```

<hr>

The comparison operators work with tuples and other sequences. Python starts by comparing the first element from each sequence. If they are equal, it goes on to the next element, and so on, until it finds elements that differ. Subsequent elements are not considered

```py
print((0, 1, 2) < (0, 3, 4))
# True

print((0, 1, 2000000) < (0, 3, 4))
# True

print((1, 1, 2) < (0, 3, 4))
# False

print((0, 3, 4) < (0, 3, 4))
# False
```

<hr>

### Logical Operators

There are three logical operators: `and`, `or`, and `not`.

```py
x = 5
print(x > 0 and x < 10) # True

x = 11
print(x > 0 and x < 10) # False
```

The `not` operator negates a boolean expression:

```py
x = 1
y = 2

print(x > y)
# False

print(not (x > y))
# True
```

<hr>

### `if` statement

The simplest form of a conditional statement is the `if` statement. The boolean expression after the `if` statement is called the condition. We end the `if` statement with a colon character (`:`) and the line(s) after the `if` statement are **indented**.

```py
x = 1

if x > 0:
  print("x is positive")
```

The `if` statement could be written in a shorter form:

```py
x = 1

if x > 0: print("x is positive")
```

When the `if` statement stretches across more than one line, it is called compound statement:

```py
x = 1
y = 0

if x > y:
  print("x is greater than y")
  print(x)
  print(y)
```

There is no limit on the number of statements that can appear in the body, but there must be at least one. Occasionally, it is useful to have a body with no statements (usually as a placeholder for code you haven’t written yet). In that case, you can use the `pass` statement to pass the Python interpreter check, which does nothing.

```py
x = -1

if x < 0 :
  pass   # need to handle negative values, do nothing for now.
```

We can also provide some alternative execution options for the `if` statement using `else`:

```py
x = 1

if x % 2 == 0:
  print('x is even')
else:
  print('x is odd')
```

Instead of providing a single alternative execution with `else`, we can use `elif` ("else if") to provide more conditions to the `if` statement:

```py
x = 1
y = 0

if x < y:
  print('x is less than y')
elif x > y:
  print('x is greater than y')
else:
  print('x and y are equal')
```

<hr>
<hr>

## Error Handling

There is a conditional execution structure built into Python to handle expected and unexpected errors called `try` / `except`. The `except` block is ignored if there is no error.

```py
numInp = input("Please provide a number\n")

try:
  integer = int(numInp)
  print(f"Your integer is {integer}")
except:
  print("You didn't provide a number")
```

The `exit` function terminates the program. It might be useful in the `except` block:

```py
numberInput = input("Please provide a number\n")

try:
  integer = int(numberInput)
  print(integer)
except:
  print("You didn't provide a number")
  exit()
```

We can specify the type of error in the `except` block, if we want to suppress only a certain type of error. Below code only suppresses the `ValueError`:

```py
def attempt_float(x):
  try:
    return float(x)
  except ValueError:
    print("ValueError")
    return x

print(attempt_float('something'))
# ValueError
# something

print(attempt_float((1, 2))) # throws an error
# TypeError: float() argument must be a string or a real number, not 'tuple'
```

You can catch multiple exception types by writing a tuple of exception types instead (the parentheses are required):

```py
def attempt_float(x):
  try:
    return float(x)
  except (ValueError, TypeError):
    print("Error")
    return x

print(attempt_float('something'))
# Error
# something

print(attempt_float((1, 2)))
# Error
# (1, 2)
```

We might want some code to be executed regardless of whether or not the code in the `try` block succeeds. To do this, use `finally`:

```py
numInp = input("Please provide a number\n")

try:
  integer = int(numInp)
  print(f"Your integer is {integer}")
except:
  print("You didn't provide a number")
finally:
  print("Thanks for the input")
```

You can use the `else` statement with `try` which will run only if the `try` block succeeds:

```py
numberInput = input("Please provide a number\n")

try:
  integer = int(numberInput)
  print(integer)
except:
  print("You didn't provide a number")
else:
  print('No errors')
finally:
  print("Thanks for the input")
```

### `raise`

The `raise` statement allows to force a specified exception to occur. The sole argument to `raise` indicates the exception to be raised. This must be either an exception instance or an exception class:

```py
def isInCaps(text):
  if text == text.upper():
    return True
  else:
    raise NameError

print(isInCaps("HELLO")) # True
print(isInCaps("Hello")) # NameError
```

We can also define the text to print to the user:

```py
def isInt(integer):
  if type(integer) == int:
    return True
  else:
    raise TypeError("Only integer")

print(isInt(2)) # True
print(isInt("HELLO")) # TypeError: Only integer
```

<hr>
<hr>

## Functions

### Creating a Function

To create a function, we use the `def` keyword:

```py
# define a function
def func():
  print("this is a function")

# call the function
func() # this is a function
```

Here is how to define a function with a parameter:

```py
def func(param):
  print(param)

func("some argument")
# some argument
```

<hr>

#### `return`

To return a result from a function, we use the `return` statement in our function:

```py
def addTwo(a, b):
  added = a + b
  return added

print(addTwo(2, 3)) # 5
```

The function (void function) that doesn't return anything returns `None`:

```py
def func(param):
  print(param)

variable = func("some argument")
print(variable)
# some argument
# None
```

<hr>

#### Positional and Keyword arguments

Each function can have positional arguments and keyword arguments. Keyword arguments are most commonly used to specify default values or optional arguments.

```py
def func(x, y, z=10):
  if z != 10:
    return z * (x + y)
  else:
    return z / (x + y)

print(func(2, 3)) # 2 = 10 / (2 + 3)
print(func(2, 3, z=5)) # 25 = 5 * (2 + 3)
```

You can pass values to the keyword argument with or without the equality sign provided, though using the equality sign is encouraged. The main restriction on function arguments is that the keyword arguments must follow the positional arguments (if any):

```py
def func(x, y, z=10):
  if z != 10:
    return z * (x + y)
  else:
    return z / (x + y)

print(func(2, 3, 5)) # 25
print(func(2, 3, z = 5)) # 25
```

<hr>

#### Assigning variables outside of a function with `global`

Variable scope is called as namespace in Python. The local namespace is created when the function is called and after the function is finished, the local namespace is destroyed (with some exceptions). Assigning variables outside of the function's scope is possible, but those variables must be declared explicitly using the `global` keyword:

```py
def func():
  a = 1
  print(a)

func() # 1
print(a) # this throws an error, because `a` is not accesible outside of the function
```

```py
def func():
  global a
  a = 1
  print(a)

func() # 1
print(a) # 1
```

```py
a = 0

def func():
  global a
  a = 1
  print(a)

func() # 1
print(a) # 1
```

<hr>

### Lambda functions

Python has support for so-called **anonymous** or **lambda** functions. This is a way of writing functions consisting of a single statement which result in the return value. They are defined with the `lambda` keyword, which has no meaning other than “we are declaring an anonymous function”.

By using the lambda functions, we can write the functions in a different, succint way:

```py
def func(val):
  return val * 2

print(func(5)) # 10
```

We can write this:

```py
func = lambda x: x * 2

print(func(5)) # 10
```

We can also create and immediately invoke lambda functions:

```py
print(
  (lambda x: x * 2)(5)
) # 10
```

Lambda functions can work with more than one parameter, as well:

```py
addStuff = lambda x, y: x + y

print(addStuff(2, 3)) # 5
```

We can also create keyword arguments with lambda functions:

```py
addStuff = lambda x, y, z=10: x + y + z

print(addStuff(2, 3)) # 15
print(addStuff(2, 3, 5)) # 10
```

<hr>

### `*args` and `**kwargs`

We can access all the position and keyword arguments of a function by using the `*args` and `**kwargs` parameters:

```py
def func(*args, **kwargs):
  print("args: ", args)
  print("kwargs: ", kwargs)

func(1, 2, 3, a=4, b=5)
"""
args:  (1, 2, 3)
kwargs:  {'a': 4, 'b': 5}
"""
```

The words `args` and `kwargs` don't really matter. The use of the `*` and `**` are crucial:

```py
def func(*anyWord, **anotherWord):
  print("anyWord: ", anyWord)
  print("anotherWord: ", anotherWord)

func(1, 2, 3, a=4, b=5)
"""
anyWord:  (1, 2, 3)
anotherWord:  {'a': 4, 'b': 5}
"""
```

When calling functions, we can also benefit from the use of the `*` and `**` operator to unpack collections of arguments into separate positional or keyword arguments respectively:

```py
def func(one, two, three):
  print(one, two, three)

func(*["Here", "we"], **{"three": "go"}) # Here we go
```

<hr>

### Decorators

Decorators are functions that wrap around other functions, allowing for the execution of extra code before and/or after the inner function executes, thus decorating it. This is ideal when you need to extend the functionality of functions that you don't want to modify. To use a decorator, we place it above the function or method.

Here is an example that doesn't use the decorator syntax, but does the same thing as a decorator does:

```py
# this function returns a function that wraps another function
def decorator(func):
    def wrapper():
        print("Something is happening before the function is called.")
        func()
        print("Something is happening after the function is called.")
    return wrapper

# define a function to be wrapped
def say_whee():
    print("Whee!")

# reassign the function so that it is wrapped
say_whee = decorator(say_whee)

# now when the wrapped/decorated function is called, something happens before and after the output of the function
say_whee()
"""
Something is happening before the function is called.
Whee!
Something is happening after the function is called.
"""
```

Instead of the above way of decorating a function, Python allows you to use decorators in a simpler way with the `@` symbol, sometimes called the pie syntax. Here is an example that uses the `@` symbol, and does the same as the above code example:

```py
def decorator(func):
    def wrapper():
        print("Something is happening before the function is called.")
        func()
        print("Something is happening after the function is called.")
    return wrapper

@decorator
def say_whee():
    print("Whee!")

say_whee()
"""
Something is happening before the function is called.
Whee!
Something is happening after the function is called.
"""
```

Python has some built-in decorators. One of them is `@classmethod`. The `@classmethod` decorator modifies a method function so that it receives the class object as the first parameter instead of an instance of the class. This method function wil have access to the class object itself.

```py
class Person:
    population = 0

    def __init__(self, name):
        self.name = name
        Person.population += 1

    @classmethod
    def get_population(cls):
        return cls.population

# Creating instances
p1 = Person("Alice")
p2 = Person("Bob")

# Calling the class method
print(Person.get_population())  # Output: 2
```

There is also `@staticmethod` decorator. It doesn't operate on instance or class directly. It doesn't have self or cls parameter.

```py
class Person:
    population = 0

    def __init__(self, name):
        self.name = name
        Person.population += 1

    # Instance method
    def say_hello(self):
        return f"Hello, my name is {self.name}."

    # Class method
    @classmethod
    def get_population(cls):
        return cls.population

    # Static method
    @staticmethod
    def is_adult(age):
        return age >= 18

# Create some instances
p1 = Person("Alice")
p2 = Person("Bob")

# Instance method (called on object)
print(p1.say_hello())          # Output: Hello, my name is Alice.

# Class method (called on class or instance)
print(Person.get_population()) # Output: 2
print(p2.get_population())     # Also works, Output: 2

# Static method (called on class or instance)
print(Person.is_adult(20))     # Output: True
print(p1.is_adult(16))         # Output: False
```

<hr>

### Some Built-in Functions

#### `max` and `min`

The `max` and `min` functions give us the largest and smallest values in a sequence, respectively:

```py
# sequence of characters
print(max("Hello World"))
print(min("Hello World"))

# a tuple
print(max(1, 2, 3))
print(min(1, 2, 3))

# a list
print(max([1, 2, 3]))
print(min([1, 2, 3]))
```

<hr>

#### `len`

`len` function tells us the length of its argument:

```py
# sequence of characters
print(len("Hello World")) # 11

# a tuple
print(len((1, 2, 3))) # 3

# a list
print(len([1, 2, 3])) # 3
```

<hr>

#### `sum`

The `sum` function returns the sum of the sequence provided to it:

```py
# a tuple
print(sum((1, 2, 3))) # 6

# a list
print(sum([1, 2, 3])) # 6
```

The `sum()` function only works when the sequence elements are numbers. The other functions (`max()`, `len()`, etc.) work with sequence of strings and other types that can be comparable.

<hr>

#### `dir`

Python has a function called `dir` which lists the attributes available for an object.

```py
text = "some text"

print(dir(text))
print(dir(int))
```

<hr>

#### `help`

You can use `help` to get some simple documentation on a method:

```py
print(help(dir))
```

<hr>

#### `range`

The `range` function generates a sequence of evenly spaced integers. A start, end, and step arguments (which may be negative) can be given to the `range` function:

```py
# only with the end argument
a = list(range(10))

print(a) # [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]

# with the start, and end arguments
b = list(range(0, 10))
c = list(range(5, 10))

print(b) # [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
print(c) # [5, 6, 7, 8, 9]

# with the start, end, and step arguments
d = list(range(0, 10, 2))
e = list(range(10, 0, -2))

print(d) # [0, 2, 4, 6, 8]
print(e) # [10, 8, 6, 4, 2]
```

<hr>

#### `enumerate`

The `enumerate` function enumerates an iterable object. Here is an example without using the `enumerate`:

```py
listVar = [1, 2, 3]

index = 0
for value in listVar:
  print(f"index: {index}, value: {value}")
  index += 1
"""
index: 0, value: 1
index: 1, value: 2
index: 2, value: 3
"""
```

With `enumerate`, we can simply do this:

```py
listVar = [1, 2, 3]

for index, value in enumerate(listVar):
  print(f"index: {index}, value: {value}")
"""
index: 0, value: 1
index: 1, value: 2
index: 2, value: 3
"""
```

Here is another simple use of `enumerate`:

```py
listVar = ["zero", "one", "three"]

print(dict(enumerate(listVar)))
# {0: 'zero', 1: 'one', 2: 'three'}
```

<hr>

#### `zip`

`zip` “pairs” up the elements of lists, tuples, or other sequences to create a list of tuples:

```py
seq1 = [1, 2, 3]
seq2 = ["one", "two", "three"]

zipped = zip(seq1, seq2)

print(list(zipped))
# [(1, 'one'), (2, 'two'), (3, 'three')]
```

`zip` can take an arbitrary number of sequences, and the number of elements it produces is determined by the shortest sequence:

```py
seq1 = [1, 2, 3]
seq2 = ["one", "two", "three"]
seq3 = [False, True]

zipped = zip(seq1, seq2, seq3)

print(list(zipped))
# [(1, 'one', False), (2, 'two', True)]
```

<hr>

#### `reversed`

`reversed` iterates over the elements of a sequence in reverse order. Keep in mind that `reversed` is a generator, so it does not create the reversed sequence until materialized (e.g., with `list` or a `for` loop):

```py
seq1 = [1, 2, 3]

print(list(seq1)) # [1, 2, 3]
```

<hr>

#### `map`

The `map` function takes a function and a sequence, and applies that function on every item of the sequence:

```py
listVar = ['one', 'two', 'three']

newList = list(map(str.capitalize, listVar))

print(newList) # ['One', 'Two', 'Three']
```

<hr>

#### `filter`

The `filter` built-in function takes a function and an iterable as arguments. It applies the function to each item in the iterable and returns a new iterable containing only the items for which the function returns `True`.

```py
def is_even(x):
    return x % 2 == 0

numbers = [1, 2, 3, 4, 5, 6]

even_numbers = list(filter(is_even, numbers))

print(even_numbers)  # [2, 4, 6]
```

<hr>
<hr>

## Generators

A generator is a convenient way to construct a new iterable object. Whereas normal functions execute and return a single result at a time, generators can return a sequence of multiple values by pausing and resuming execution each time the generator is used. To create a generator, use the `yield` keyword instead of `return` in a function:

```py
def squares(n = 10):
  print(f"Generating squares from 1 to {n ** 2}")
  for i in range(n + 1):
    yield i ** 2
```

When you actually call the generator, no code is immediately executed. It is not until you request elements from the generator that it begins executing its code:

```py
def squares(n = 10):
  print(f"Generating squares form 1 to {n ** 2}")
  for i in range(n + 1):
    yield i ** 2

gen = squares()
print(gen) # <generator object squares at 0x0000019FE40A92A0>

for x in gen:
  print(x, end=", ")
"""
Generating squares from 1 to 100
0, 1, 4, 9, 16, 25, 36, 49, 64, 81, 100,
"""
```

Another way to make a generator is by using a generator expression. This is a generator analogue to list, dictionary, and set comprehensions. To create one, enclose what would otherwise be a list comprehension within parentheses instead of brackets:

```py
gen = (x ** 2 for x in range(10))

print(gen) # <generator object squares at 0x0000019FE40A92A0>

for i in gen:
  print(i)
```

The above is the equivalent of this:

```py
def _make_gen():
  for x in range(10):
    yield x ** 2

gen = _make_gen()

for i in gen:
  print(i)
```

<hr>
<hr>

## Loops

### `while` loop

Here is how to define a `while` loop in Python:

```py
n = 5
while n > 0:
  print(n)
  n = n - 1

print("Loop ended")
```

Instead of incrementing `n` using `n = n - 1`, `n = n + 1`, we can use `n -= 1`, `n += 1`, etc.

<hr>

### `for` loop

`for` loops are for iterating over a collection (like a list or tuple) or an iterater.

Here is an example of a `for` loop:

```py
listVar = ["item 1", "item 2", "item 3"]

for item in listVar:
  print(item)

print("Done")
"""
item 1
item 2
item 3
Done
"""
```

In the same manner, we can loop through a string:

```py
for char in "word":
  print(char)
```

<hr>

### `break` statement

To manually break the loop, we use the `break` statement:

```py
n = 5
while n > 0:
  print(n)
  n = n - 1
  if (n == 3):
    break

print("Loop ended")
"""
5
4
Loop ended
"""
```

The `break` keyword only terminates the innermost loop; any outer loops will continue to run:

```py
for outer in range(3):
  for inner in range(3):
    if inner > outer:
      print("")
      break
    print(f"outer: {outer}, inner: {inner}")
"""
outer: 0, inner: 0

outer: 1, inner: 0
outer: 1, inner: 1

outer: 2, inner: 0
outer: 2, inner: 1
outer: 2, inner: 2
"""
```

<hr>

### `continue` statement

You can use the `continue` statement to skip to the next iteration without finishing the body of the loop for the current iteration:

```py
n = 4
while n > 0:
  n -= 1
  if (n == 2):
    continue
  print(n)

print("Loop ended")
"""
3
1
0
Loop ended
"""
```

<hr>
<hr>

## `random` module

The `random` module provides functions that generate pseudorandom numbers. Before we can use the module, we have to import it:

```py
import random
```

The function `random` returns a random float between 0.0 and 1.0 (including 0.0 but not 1.0).

```py
import random

print(random.random())
```

The function `randint` takes the parameters low and high, and returns an integer between low and high (including both).

```py
import random

print(random.randint(0, 10))
print(random.randint(1, 100))
```

To choose an element from a sequence at random, you can use `choice`:

```py
import random

nums = [1, 2, 3]

print(random.choice(nums))
print(random.choice(nums))
```

<hr>
<hr>

## `math` module

Python has a `math` module that provides most of the familiar mathematical functions. Before we can use the module, we have to import it:

```py
import math
```

The expression `math.pi` gets the variable pi from the `math` module. The value of this variable is an approximation of π, accurate to about 15 digits.

```py
import math

print(math.pi) # 3.141592653589793
```

`sqrt` returns the square root of a number:

```py
import math

print(math.sqrt(4)) # 2.0
```

`pow` takes base and power as arguments and raises the base to the power:

```py
import math

base = 5
exponent = 2

print(math.pow(base, exponent)) # 25.0
```

<hr>
<hr>

## `os` module

We can use various methods provided in the `os` module to get the information about the operating system. Before we can use the module, we have to import it:

```py
import os
```

<hr>

### `getcwd()`

The `getcwd()` method provides the link of the current working directory (where the python runs):

```py
import os

print(os.getcwd())
```

<hr>

### `listdir()`

The `listdir()` method lists the files in a directory:

```py
import os

# lists the files in the directory where the python runs
print(os.listdir())

# lists the files in the provided relative path
print(os.listdir("./practice"))

# lists the files in the provided absolute path
print(os.listdir("c:/Users/ZiyaA/Downloads"))
```

Because the `listdir()` method returns a list, we can use it with the `in` operator, to check if a certain folder exists in some directory.

<hr>

### `makedirs()`

The `makedirs()` method creates a new directory. If `exist_ok=True`, then it won't throw an exception when the folder already exists and it won't override the existing folder:

```py
import os

os.makedirs("./newFolder", exist_ok=True)
```

<hr>
<hr>

## Working with Files

### `open` function

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

<hr>

### Using the `with` keyword

It is good practice to use the `with` keyword when dealing with file objects. The advantage is that the file is properly closed after the job is done, even if an exception is raised at some point.

```py
import os

file_path = os.path.join(os.getcwd(), "text.txt")

with open(file_path, encoding="utf-8") as fhand:
  for line in fhand:
    print(str.rstrip(line))
```

If you’re not using the `with` keyword, then you should call `close()` to close the file and immediately free up any system resources used by it.

<hr>

### `closed` property

We can check that the file has been closed using the `closed` property on the file handle.

```py
import os

file_path = os.path.join(os.getcwd(), "text.txt")

with open(file_path, encoding="utf-8") as fhand:
  for line in fhand:
    print(str.rstrip(line))

print(fhand.closed) # True
```

<hr>

### Reading files with the `read` method

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

<hr>

### Reading files with the `readline` method

`readline()` reads a single line from the file; a newline character (`\n`) is left at the end of the string, and is only omitted on the last line of the file if the file doesn’t end in a newline.

```py
import os

file_path = os.path.join(os.getcwd(), "text.txt")

with open(file_path, encoding="utf-8") as fhand:
  text = fhand.readline()

print(len(text))
print(text)
```

<hr>

### Opening files in `"w"` mode and writing with the `write` method

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

<hr>

Other types of objects need to be converted – either to a string (in text mode) or a bytes object (in binary mode) – before writing them:

```py
import os

file_path = os.path.join(os.getcwd(), "text.txt")

tup = ("hello", 2, "you")

with open(file_path, "w", encoding="utf-8") as fhand:
  stringified = str(tup)
  fhand.write(stringified)
```

<hr>

### Opening files in `"x"` mode

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

<hr>

### Opening files in `"a"` mode

The `"a"` mode appends to the file. It creates the file if it does not already exist:

```py
import os

file_path = os.path.join(os.getcwd(), "text2.txt")

with open(file_path, "a", encoding="utf-8") as fhand:
  fhand.write("\nSome more data for the file.")

with open(file_path, encoding="utf-8") as fhand:
  print(fhand.read()) # Here is some text.
```

<hr>

### Opening files in `"r+"` mode

The `"r+"` mode returns a file handle that could be used both to read from and write to the file:

```py
import os

file_path = os.path.join(os.getcwd(), "text.txt")

with open(file_path, "r+", encoding="utf-8") as fhand:
  fhand.write("This is to be written into the file.")
  print(fhand.read()) # This is to be written into the file.
```

<hr>

In addition to the above modes, you can specify if the file should be handled as binary or text mode using the `"t"` and `"b"` flags. `"rt"` is the default value. So, if no mode is specified with the `open` function, these are going to be assumed.

<hr>
<hr>

## Lists

Like a string, a list is a sequence of values. In a string, the values are characters; in a list, they can be any type. The values in lists are called elements or sometimes items.

<hr>

### Creating a list

There are several ways to create a new list; the simplest is to enclose the elements in square brackets (“[” and ”]”):

```py
# list of integers
[10, 20, 30, 40]

# list of strings
['item 1', 'item 2', 'item 3']

# list of different data types
['some list item', 2.0, 5, [10, 20]]

# a list assigned to a variable
listVariable = ['item 1']
```

Another way to create a list item is to use the `list` function. If no argument is provided, it creates an empty list. If the argument is provided, the argument should be an iterable object, like a tuple or string:

```py
print(list()) # []

listVar = list("text")

print(listVar) # ['t', 'e', 'x', 't']
```

### Accessing list items

We can access the list items using the square bracket notation:

```py
listVariable = [1, 2, 3, 4]

print(listVariable[0]) # 1
print(listVariable[1:3]) # [2, 3]
print(listVariable[:]) # [1, 2, 3, 4]
```

If an index provided to the bracket notation has a negative value, it counts backward from the end of the list.

```py
listVariable = [1, 2, 3, 4]

print(listVariable[-1]) # 4
print(listVariable[-2]) # 3
```

We have so far used the slicing notation with `[start:stop]`. We can also use the third item, which is step, with the slice notation, to indicate which elements should be accessed:

```py
listVariable = [1, 2, 3, 4, 5, 6, 7, 8, 9]

# every second element from index 1 to 8
print(listVariable[1:8:2]) # [2, 4, 6, 8]

# every third element from index 1 to the end of the list
print(listVariable[1::3]) # [2, 5, 8]
```

A clever use of this is to pass -1, which has the useful effect of reversing a list.

```py
listVariable = [1, 2, 3, 4, 5, 6, 7, 8, 9]

print(listVariable[::-1]) # [9, 8, 7, 6, 5, 4, 3, 2, 1]
```

We can also assign items to a specific position in a list using the bracket notation:

```py
listVariable = [1, 2, 3, 4]

print(listVariable[0]) # 1

listVariable[0] = 5
print(listVariable[0]) # 5

listVariable[1:3] = [6, 7]
print(listVariable) # [5, 6, 7, 4]
```

<hr>

### Using the `in` operator with lists

The `in` operator also works on lists.

```py
listVariable = ['item 1', 'item 2', 'item 3']

print('item 1' in listVariable) # True
print('item 4' in listVariable) # False
```

The keyword `not` can be used to negate `in`:

```py
listVariable = ['item 1', 'item 2', 'item 3']

print('item 1' not in listVariable) # False
print('item 4' not in listVariable) # True
```

<hr>

### Looping through lists with the `for` loop

To traverse the list, we can use the `for` loop. However, to update the items in a list, we need indices as well. To have both indices and traverse the list, we can use the `range` function:

```py
numbers = [1, 2, 3, 4]

for i in range(len(numbers)):
  numbers[i] = numbers[i] ** 2

print(numbers) # [1, 4, 9, 16]
```

A `for` loop over an empty list never executes the body:

```py
empty = []

for x in empty:
  print('This never happens.')
```

<hr>

### Using `+` and `*` operators with lists

The `+` operator used on two and more lists, concatenates those lists:

```py
a = [1, 2, 3]
b = [4, 5, 6]
c = a + b

print(c)
# [1, 2, 3, 4, 5, 6]
```

We can also use the `+` operator to add to an existing list:

```py
listVar = [1, 2, 3]
listVar = listVar + [4]

print(listVar) # [1, 2, 3, 4]
```

The `*` operator repeats a list a given number of times:

```py
print([0] * 4)
# [0, 0, 0, 0]

print([1, 2, 3] * 3)
# [1, 2, 3, 1, 2, 3, 1, 2, 3]
```

<hr>

### List Methods

Most list methods are void; they modify the list and return `None`.

<hr>

#### `append`

The `append` method adds a new element to the end of a list:

```py
listVar = ['a', 'b', 'c']
listVar.append('d')

print(listVar) # ['a', 'b', 'c', 'd']
```

<hr>

#### `extend`

The `extend` method takes a list as an argument and appends all of the elements:

```py
listVar1 = ["a", "b", "c"]
listVar2 = ["d", "e"]
listVar1.extend(listVar2)

print(listVar1) # ['a', 'b', 'c', 'd', 'e']
```

<hr>

#### `insert`

Using `insert` you can insert an element at a specific location in the list:

```py
listVar = [1, 2, 3, 4]
listVar.insert(2, 'three')

print(listVar) # [1, 2, 'three', 3, 4]
```

<hr>

#### `sort`

The `sort` method arranges the elements of the list from low to high:

```py
listVar = ['d', 'c', 'e', 'b', 'a']
listVar.sort()

print(listVar) # ['a', 'b', 'c', 'd', 'e']
```

To sort in the reverse order, we can use `.sort(reverse=True)`:

```py
listVar = ['d', 'c', 'e', 'b', 'a']
listVar.sort(reverse=True)

print(listVar) # ['e', 'd', 'c', 'b', 'a']
```

`sort` has a few options that will occasionally come in handy. One is the ability to pass a secondary sort key—that is, a function that produces a value to use to sort the objects.

```py
listVar = ["saw", "small", "He", "foxes", "six"]
listVar.sort(key=len)

print(listVar)
```

#### The `sorted` function

The `sorted` function returns a new sorted list from the elements of any sequence. It doesn't modify the original list:

```py
listVar = ['d', 'c', 'e', 'b', 'a']
newList = sorted(listVar)

print(listVar) # ['d', 'c', 'e', 'b', 'a']
print(newList) # ['a', 'b', 'c', 'd', 'e']
```

Unlike the `sort` method, the `sorted` function also works on strings.

```py
stringVar = 'hello'

print(sorted(stringVar)) # ['e', 'h', 'l', 'l', 'o']
```

<hr>

#### `reverse`

The `reverse` method reverses the list in place:

```py
listVar = [1, 2, 3, 4]
listVar.reverse()

print(listVar) # [4, 3, 2, 1]
```

<hr>

### Deleting List Elements

If you know the index of the element you want to delete, you can use the `pop` method. `pop` modifies the list and returns the element that was removed. If you don’t provide an index, it deletes and returns the last element:

```py
listVar = ['a', 'b', 'c']
deletedItem = listVar.pop(1)

print(listVar) # ['a', 'c']
print(deletedItem) # b

lastItem = listVar.pop()

print(listVar) # ['a']
print(lastItem) # c
```

If you don’t need the removed value, you can use the `del` statement:

```py
listVar = ['a', 'b', 'c']

del listVar[1]

print(listVar) # ['a', 'c']
```

To remove more than one element, you can use `del` with slice indexing:

```py
listVar = ['a', 'b', 'c', 'd', 'e', 'f']

del listVar[1:5]

print(listVar) # ['a', 'f']
```

If you know the element you want to remove (but not the index), you can use the `remove` method. The return value from `remove` is `None`:

```py
listVar = ['a', 'b', 'c', 'd', 'e', 'f']

listVar.remove('c')

print(listVar) # ['a', 'b', 'd', 'e', 'f']
```

<hr>
<hr>

## Dictionaries

A dictionary is like a list, but more general. In a list, the index positions have to be integers; in a dictionary, the indices can be (almost) any type. You can think of dictionaries as the mapping between keys and values.

<hr>

### Creating a dictionary

The function `dict` creates a new dictionary with no items.

```py
dictionaryItem = dict()

print(dictionaryItem) # {}
```

We can also create a dictionary using curly braces:

```py
eng2sp = {'one': 'uno', 'two': 'dos', 'three': 'tres'}

print(eng2sp)
# {'one': 'uno', 'two': 'dos', 'three': 'tres'}
```

<hr>

### Accessing dictionary items

We use the keys to look up the corresponding values in a dictionary:

```py
eng2sp = {'one': 'uno', 'two': 'dos', 'three': 'tres'}

print(eng2sp['two']) # 'dos'
```

<hr>

### Adding dictionary items

Here is how add items to a dictionary, after creating it:

```py
eng2sp = dict()

eng2sp['one'] = 'uno'

print(eng2sp) # {'one': 'uno'}
```

<hr>

### Using `len` function on dictionaries

The `len` function works on dictionaries; it returns the number of key-value pairs:

```py
eng2sp = {'one': 'uno', 'two': 'dos', 'three': 'tres'}

print(len(eng2sp)) # 3
```

<hr>

### Using `in` operator with dictionaries

The `in` operator works on dictionaries; it tells you whether something appears as a key in the dictionary:

```py
eng2sp = {'one': 'uno', 'two': 'dos', 'three': 'tres'}

print('one' in eng2sp) # True
print('uno' in eng2sp) # False
```

<hr>

### The `values` method

To get all the values in a dictionary, we can use the `values` method:

```py
eng2sp = {'one': 'uno', 'two': 'dos', 'three': 'tres'}

vals = list(eng2sp.values())
print(vals) # ['uno', 'dos', 'tres']

print('uno' in vals) # True
```

<hr>

### The `keys` method

In addition to `values` method, there is also `keys` method available in dictionary objects:

```py
eng2sp = {'one': 'uno', 'two': 'dos', 'three': 'tres'}

keysInDictionary = list(eng2sp.keys())
print(keysInDictionary) # ['one', 'two', 'three']
```

<hr>

### The `items` method

Dictionaries have a method called `items` that returns a list of tuples, where each tuple is a key-value pair:

```py
d = {'b':1, 'a':10, 'c':22}
t = list(d.items())

print(t) # [('b', 1), ('a', 10), ('c', 22)]
```

Combining the `items` method, tuple assignment, and `for`, could help us traverse the keys and values of a dictionary in a single loop:

```py
d = {'a':10, 'b':1, 'c':22}

for key, val in d.items():
  print(key, val)
```

<hr>

### `get`

Dictionaries have a method called `get` that takes a key and a default value. If the key appears in the dictionary, `get` returns the corresponding value; otherwise it returns the default value.

```py
dictionary = {'one': 1, 'two': 2, 'three': 3}

print(dictionary.get('one', 1)) # 1
print(dictionary.get('two', 10)) # 2
print(dictionary.get('four', 4)) # 4
```

<hr>

### `update`

You can merge one dictionary into another using the `update` method:

```py
dictionary = {"one":1, "two": 2, "three": 3}

dictionary.update({"four": 4})

print(dictionary) # {'one': 1, 'two': 2, 'three': 3, 'four': 4}
```

The `update` method changes dictionaries in place, so any existing keys in the data passed to `update` will have their old values discarded.

```py
dictionary = {"one":1, "two": 2, "three": 3}

dictionary.update({"three": 33 })

print(dictionary) # {'one': 1, 'two': 2, 'three': 33}
```

<hr>

### Looping through dictionary items

To loop through the dictionary, we can use the `for` loop:

```py
dictionary = {'one': 1, 'two': 2, 'three': 3}

for key in dictionary:
  print(key, dictionary[key])
```

<hr>

### Deleting items from a dictionary

You can delete values in a dictionary using the `del` keyword:

```py
dictionary = {"one":1, "two": 2, "three": 3}

del dictionary["one"]

print(dictionary) # {'two': 2, 'three': 3}
```

The `pop` method simultaneously returns the value and deletes the key:

```py
dictionary = {"one":1, "two": 2, "three": 3}

popped = dictionary.pop("one")

print(popped) # 1
print(dictionary) # {'two': 2, 'three': 3}
```

<hr>

### Dictionary unpacking with `**`

The `**` operator is called the dictionary unpacking operator.

```py
numbers = {"one": 1, "two": 2, "three": 3}
letters = {"a": "A", "b": "B", "c": "C"}
combination = {**numbers, **letters}

print(combination)
# {'one': 1, 'two': 2, 'three': 3, 'a': 'A', 'b': 'B', 'c': 'C'}
```

If the dictionaries we're trying to merge have repeated or common keys, then the values of the right-most dictionary will override the values of the left-most dictionary.

```py
numbers = {"one": 1, "two": 2, "three": 3}
numbers2 = {"one": 11, "four": 4, "three": 33}
print({**numbers, **numbers2})
# {'one': 11, 'two': 2, 'three': 33, 'four': 4}
```

<hr>
<hr>

## Tuples

Syntactically, a tuple is a comma-separated list of values. The values stored in a tuple can be any type, and they are indexed by integers. The important difference is that tuples are **immutable**. Tuples are also comparable and hashable so we can sort lists of them and use tuples as key values in Python dictionaries.

<hr>

### Creating a tuple

Here is an example of creating a tuple:

```py
t = 'a', 'b', 'c'

print(type(t)) # <class 'tuple'>
print(t) # ('a', 'b', 'c')
```

Although it is not necessary, it is common to enclose tuples in parentheses to help us quickly identify tuples when we look at Python code:

```py
t = ("a", "b", "c")

print(type(t)) # <class 'tuple'>
```

To create a tuple with a single element, you have to include the final comma:

```py
t1 = ("a",)
t2 = "a",
t3 = "a"

print(type(t1)) # <class 'tuple'>
print(type(t2)) # <class 'tuple'>
print(type(t3)) # <class 'str'>
```

Another way to construct a tuple is the built-in function `tuple`. With no argument, it creates an empty tuple:

```py
t = tuple()
print(t) # ()
```

If the argument to the `tuple` is a sequence (string, list, or tuple), the result of the call is a tuple with the elements of the sequence:

```py
t = tuple('text')
print(t) # ('t', 'e', 'x', 't')

print(tuple([4, 0, 2])) # (4, 0, 2)
```

<hr>

### Accessing tuple elements

We can access the elements in a tuple using the square bracket syntax:

```py
t = ('a', 'b', 'c', 'd', 'e')

print(t[0]) # 'a'
print(t[1:3]) # ('b', 'c')
```

<hr>

### Some possible modifications in a tuple

You can’t modify the elements of a tuple, but you can replace one tuple with another:

```py
t = ('a', 'b', 'c', 'd', 'e')
t = ('A',) + t[1:]

print(t) # ('A', 'b', 'c', 'd', 'e')
```

If an object inside a tuple is mutable, such as a list, you can modify it in place. While the objects stored in a tuple may be mutable themselves, once the tuple is created it’s not possible to modify which object is stored in each slot:

```py
tup = tuple(['foo', [1, 2], True])

print(tup[1]) # [1, 2]

tup[1].append(3)
print(tup) # ('foo', [1, 2, 3], True)

# this one throws an error
tup[2] = False
```

<hr>

### Using `+` and `*` operators with tuples

You can concatenate tuples using the `+` operator to produce longer tuples:

```py
t1 = (4, None, 'foo')
t2 = (6, 0)
t3 = t1 + t2 + ('bar',)

print(t3) # (4, None, 'foo', 6, 0, 'bar')
```

Multiplying a tuple by an integer, as with lists, has the effect of concatenating that many copies of the tuple:

```py
t = ('foo', 'bar') * 4

print(t) # ('foo', 'bar', 'foo', 'bar', 'foo', 'bar', 'foo', 'bar')
```

<hr>

### `count`

The `count` method, counts the number of occurrences of a value in a tuple:

```py
t = (1, 2, 2, 2, 3, 4, 2)

t.count(2) # 4

# `count` also works on strings and lists
"hello".count("l") # 2
[1, 2, 2, 2, 3, 4, 2].count(2) # 2
```

<hr>
<hr>

## Iterable Unpacking

In this example, we have a two-element tuple. We assign the first and second elements of the tuple to the variables `first` and `second` in a single statement.

```py
tup = ("first", "second")
first, second = tup

print(first) # 'first'
print(second) # 'second'
```

The left side of the above assignment is a tuple, as well. So, below example is valid as above one:

```py
tup = ("first", "second")
(first, second) = tup

print(first) # 'first'
print(second) # 'second'
```

If the right side of the assignmen is an iterable this unpacking syntax would work. Here is an example with a two-element list:

```py
listVar = ["first", "second"]
first, second = listVar

print(first) # 'first'
print(second) # 'second'
```

Here is one more example:

```py
email = "address@example.org"
username, domain = email.split("@")

print(username) # address
print(domain) # example.org
```

We can easily swap the values of variables using this syntax:

```py
a = 0
b = 1

a, b = b, a

print(a) # 1
print(b) # 0
```

The number of variables on the left and the number of values on the right must be the same:

```py
a, b = 1, 2, 3
# ValueError: too many values to unpack
```

If we want to avoid having this error, but are not sure how many values will be on the right side, we can use the `*` to pack several values in a single variable:

```py
a, b, *c = 1, 2, 3, 4, 5
print(a) # 1
print(b) # 2
print(c) # [3, 4, 5]

a, *b, c = 1, 2, 3, 4, 5

print(a) # 1
print(b) # [2, 3, 4]
print(c) # 5
```

<hr>

A common use of iterable unpacking is iterating over sequences of tuples or lists:

```py
seq = [(1, 2, 3), (4, 5, 6), (7, 8, 9)]

for a, b, c in seq:
  print(f'a={a}, b={b}, c={c}')
"""
a=1, b=2, c=3
a=4, b=5, c=6
a=7, b=8, c=9
"""
```

<hr>
<hr>

## Classes

In Python, **attributes** are variables defined inside a class. **Methods** are functions that you define within a class. Attributes and methods are collectively referred to as **members** of a class or object.

<hr>

### Creating a class and an object instance

- To define a class, you need to use the `class` keyword followed by the class name and a colon.
- The `.__init__()` method, inside classes, is known as the object initializer because it defines and sets the initial values for your attributes.
- The first argument of the most methods is `self`. This argument holds a reference to the current object so that you can use it inside a class.

Here is an example of creating a class:

```py
class ClassName:
  def __init__(self, someVariable):
    self.someVariable = someVariable
    self.anotherVariable = 'some data'

  def printData(self):
    print(self.someVariable)
```

Here is how we create an object instance from a class constructor:

```py
newObj = ClassName("something")
newObj.printData() # something
print(newObj.anotherVariable) # some data

newObj2 = ClassName("another thing")
newObj2.printData() # another thing
print(newObj2.anotherVariable) # some data
```

<hr>

### Accessing class members with `getattr`

Attributes and methods can also be accessed by name via the `getattr` function:

```py
class ClassName:
  def __init__(self, someVariable):
    self.someVariable = someVariable
    self.anotherVariable = 'some data'

  def printData(self):
    print(self.someVariable)

  var = "variable"


print(getattr(ClassName, "printData")) # <function ClassName.printData at 0x00000287F35993A0>
print(getattr(ClassName, "var")) # variable
```

<hr>

### Name mangling and naming convention for private class members

In Python, all attributes are accessible in one way or another. However, Python has a well-established naming convention that you should use to communicate that an attribute or method isn’t intended for use from outside its containing class or object. The naming convention consists of adding a leading underscore to the member’s name. A variable named `_variable` in a class is a non-public variable.

Another naming convention that you need to take into account in Python classes is adding two leading underscores to attribute and method names. This naming convention triggers what’s known as **name mangling**. Name mangling is an automatic name transformation that prepends the class’s name to the member’s name. For example, `__attribute` becomes `_ClassName__attribute` or `__method` becomes `_ClassName__method`. It’s a way to avoid naming conflicts between classes or subclasses.

```py
class ClassName:
  def __init__(self, someVariable):
    self.someVariable = someVariable

  def __some_method(self):
    return print(self.someVariable)

newObj = ClassName("Hello")
newObj._ClassName__some_method() # Hello
newObj.__some_method() # AttributeError: 'ClassName' object has no attribute '__some_method'
```

<hr>

### Class attributes vs instance attributes

In Python, there are instance and class attributes.

**Instance attributes** are shared between different instances of a class and they are accessed using `self` inside the class. The `self` argument holds a reference to the current instance, which is where the attributes belong and live.

In the below example, the `Car` class have several instance attributes that will be available in all the instances of the `Car` class. Note how the values of the associated attributes are different and specific to the concrete instance:

```py
class Car:
  def __init__(self, brand, year):
    # instance attributes
    self.brand = brand
    self.year = year
    self.max_speed = 200

newCar = Car("Togg", 2024)
print(newCar.brand, newCar.year, newCar.max_speed)
# Togg 2024 200

newCar2 = Car("Togg", 2020)
print(newCar2.brand, newCar2.year, newCar2.max_speed)
# Togg 2020 200
```

**Class attributes** are variables that you define directly in the class body but outside of any method. These attributes are tied to the class itself rather than to particular instances of that class. If you change a class attribute, that change affects all the derived objects.

```py
class ObjectCounter:
  # class attributes
  num_instances = 0

  def __init__(self):
    ObjectCounter.num_instances += 1

ObjectCounter()
ObjectCounter()
counter = ObjectCounter()
counter2 = ObjectCounter()

print(ObjectCounter.num_instances) # 4
print(counter.num_instances) # 4
print(counter2.num_instances) # 4
```

It’s important to note that you can access class attributes using either the class or one of its instances. That’s why you can use the `counter` object to retrieve the value of `.num_instances`. However, if you need to modify a class attribute, then you must use the class itself rather than one of its instances.

```py
class ObjectCounter:
  num_instances = 0

  def __init__(self):
    ObjectCounter.num_instances += 1

ObjectCounter()
counter = ObjectCounter()

print(ObjectCounter.num_instances) # 2
print(counter.num_instances) # 2

ObjectCounter.num_instances = 10
print(ObjectCounter.num_instances) # 10
print(counter.num_instances) # 10

counter.num_instances = 100
print(ObjectCounter.num_instances) # 10
print(counter.num_instances) # 100
```

In general, you should use class attributes for sharing data between instances of a class. Any changes on a class attribute will be visible to all the instances of that class.

<hr>

### `__dict__` attribute

In Python, both classes and instances have a special attribute called `__dict__`. This attribute holds a dictionary containing the writable members of the underlying class or instance. Remember that:

- `__dict__` used on a class shows all the class attributes and methods.
- `__dict__` used on an instance shows only the instance attributes and methods.

```py
class SampleClass:
  class_attr = 100

  def __init__(self, instance_attr):
    self.instance_attr = instance_attr

  def method(self):
    print(f"Class attribute: {self.class_attr}")
    print(f"Instance attribute: {self.instance_attr}")

print(SampleClass.__dict__)
print(SampleClass.__dict__['class_attr']) # 100
print(SampleClass.__dict__['method']) # <function SampleClass.method at 0x00000197A48493A0>

sample = SampleClass("instance")
print(sample.__dict__) # {'instance_attr': 'instance'}
```

<hr>
<hr>

## Sets

A set is an unordered collection of unique elements.

Like dictionary keys, set elements generally must be immutable, and they must be hashable (which means that calling `hash` on a value does not raise an exception). In order to store list-like elements (or other mutable sequences) in a set, you can convert them to tuples.

<hr>

### Creating sets

A set can be created in two ways: via the `set` function or via a set literal with curly braces:

```py
mySet1 = set([2, 2, 2, 1, 3, 3])
mySet2 = {2, 2, 2, 1, 3, 3}

print(mySet1) # {1, 2, 3}
print(mySet2) # {1, 2, 3}
```

<hr>

### Mathematical operations on sets

Sets support mathematical set operations like union, intersection, difference, and symmetric difference. If you pass an input that is not a set to methods like `union` and `intersection`, Python will convert the input to a set before executing the operation. When using the binary operators, both objects must already be sets.

<hr>

#### Union

The union of the two sets is the set of distinct elements occurring in either set. This can be computed with either the `union` method or the `|` binary operator:

```py
a = {1, 2, 3, 4, 5}
b = {3, 4, 5, 6, 7, 8}

c = a.union(b)
print(c) # {1, 2, 3, 4, 5, 6, 7, 8}

c = a | b
print(c) # {1, 2, 3, 4, 5, 6, 7, 8}
```

The above methods don't change the original sets. However, we can change the set to the union, using the `update` method or `|=` operator:

```py
a = {1, 2, 3, 4, 5}
b = {3, 4, 5, 6, 7, 8}

a.update(b)

print(a) # {1, 2, 3, 4, 5, 6, 7, 8}
```

```py
a = {1, 2, 3, 4, 5}
b = {3, 4, 5, 6, 7, 8}

a |= b

print(a) # {1, 2, 3, 4, 5, 6, 7, 8}
```

<hr>

#### Intersection

The intersection contains the elements occurring in both sets. This can be computed with either the `intersection` method or `&` operator:

```py
a = {1, 2, 3, 4, 5}
b = {3, 4, 5, 6, 7, 8}

c = a.intersection(b)
print(c) # {3, 4, 5}

c = a & b
print(c) # {3, 4, 5}
```

The intersection method and operator do not change the original sets. To update the original set, we can use the `intersection_update` method or `&=` operator:

```py
a = {1, 2, 3, 4, 5}
b = {3, 4, 5, 6, 7, 8}

a.intersection_update(b)

print(a) # {3, 4, 5}
```

```py
a = {1, 2, 3, 4, 5}
b = {3, 4, 5, 6, 7, 8}

a &= b

print(a) # {3, 4, 5}
```

<hr>

#### Difference

If we have two sets - `a` and `b`, we can get the elements in `a` that are not in `b` using the `difference` method or `-` operator:

```py
a = {1, 2, 3, 4, 5}
b = {3, 4, 5, 6, 7, 8}

c = a.difference(b)
print(c) # {1, 2}

c = a - b
print(c) # {1, 2}
```

To update the original set, we can use the `difference_update` method or `-=` operator:

```py
a = {1, 2, 3, 4, 5}
b = {3, 4, 5, 6, 7, 8}

a.difference_update(b)

print(a) # {1, 2}
```

```py
a = {1, 2, 3, 4, 5}
b = {3, 4, 5, 6, 7, 8}

a -= b

print(a) # {1, 2}
```

<hr>

#### Symmetric difference

To get all of the elements in the set `a` or `b`, but not in both, we can use the `symmetric_difference` method or `^` operator:

```py
a = {1, 2, 3, 4, 5}
b = {3, 4, 5, 6, 7, 8}

c = a.symmetric_difference(b)
print(c) # {1, 2, 6, 7, 8}

c = a ^ b
print(c) # {1, 2, 6, 7, 8}
```

To update the original set, we can use the `symmetric_difference_update` method or `^=` operator:

```py
a = {1, 2, 3, 4, 5}
b = {3, 4, 5, 6, 7, 8}

a.symmetric_difference_update(b)

print(a) # {1, 2, 6, 7, 8}
```

```py
a = {1, 2, 3, 4, 5}
b = {3, 4, 5, 6, 7, 8}

a ^= b

print(a) # {1, 2, 6, 7, 8}
```

<hr>

### `issubset`

We can check if the set `a` is the subset of set `b` (in other words, if all the elements of set `a` is contained within set `b`) using the `issubset` method or `<=` operator:

```py
a = {1, 2, 3, 4, 5}
b = {3, 4, 5, 6, 7, 8}
c = {1, 2, 3, 4, 5, 6, 7, 8, 9}

print(a.issubset(b)) # False
print(b.issubset(c)) # True

print(a <= b) # False
print(b <= c) # True
```

<hr>

### `issuperset`

We can check if the set `a` is the superset of set `b` (in other words, if all the elements of `b` contained within set `a`) using the `issuperset` method or `>=` operator:

```py
a = {1, 2, 3, 4, 5}
b = {3, 4, 5, 6, 7, 8}
c = {1, 2, 3, 4, 5, 6, 7, 8, 9}

print(a.issuperset(b)) # False
print(c.issuperset(b)) # True

print(a >= b) # False
print(c >= b) # True
```

<hr>

### `isdisjoint`

We can check if two sets have no common elements using the `isdisjoint` method:

```py
a = {1, 2, 3, 4, 5}
b = {6, 7, 8}

print(a.isdisjoint(b)) # True
```

<hr>

### `add`

We can add an element to a set using the `add` method:

```py
a = {1, 2, 3, 4, 5}
a.add(6)

print(a) # {1, 2, 3, 4, 5, 6}
```

<hr>

### `clear`

We can reset a set to an empty state, discarding all of its elements, by using the `clear` method:

```py
a = {1, 2, 3, 4, 5}
a.clear()

print(a) # set()
```

<hr>

### Deleting set elements

We can remove an element from a set using the `remove` method:

```py
a = {1, 2, 3, 4, 5}
a.remove(3)

print(a) # {1, 2, 4, 5}
```

We can remove the first element from a set using the `pop` method. It will raise a `KeyError` if the set is empty:

```py
a = {1, 2, 3, 4, 5}
b = a.pop()

print(a) # {2, 3, 4, 5}
print(b) # 1
```

<hr>

### Equality of sets

Sets are equal if and only if their contents are equal:

```py
print({1, 2, 3} == {3, 2, 1}) # True
```

<hr>
<hr>

## List, Set, and Dictionary Comprehensions

List comprehensions allow you to concisely form a new list by filtering the elements of a collection, transforming the elements passing the filter into one concise expression. The filter condition can be omitted, leaving only the expression. List comprehension takes the basic form:

```py
[expr for value in collection if condition]
```

For example, given a list of strings, we could filter out strings with length 2 or less and convert them to uppercase like this:

```py
strings = ["a", "as", "bat", "car", "dove", "python"]

newList = [x.upper() for x in strings if len(x) > 2]
print(newList) # ['BAT', 'CAR', 'DOVE', 'PYTHON']
```

We can also change the position of the `if` and add `else` to it:

```py
strings = ["a", "as", "bat", "car", "dove", "python"]

newList = [x.upper() if len(x) > 2 else 0 for x in strings]
print(newList) # [0, 0, 'BAT', 'CAR', 'DOVE', 'PYTHON']
```

<hr>

A set comprehension looks like the equivalent list comprehension except with curly braces instead of square brackets:

```py
set_comp = {expr for value in collection if condition}
```

Here is an example:

```py
strings = ["a", "as", "bat", "car", "dove", "python"]

unique_lengths = {len(x) for x in strings}
print(unique_lengths) # {1, 2, 3, 4, 6}
```

<hr>

A dictionary comprehension looks like this:

```py
dict_comp = {key: value for value in collection if condition}
```

Here is an example:

```py
strings = ["a", "as", "bat", "car", "dove", "python"]

newDictionary = {value: index for index, value in enumerate(strings)}
print(newDictionary) # {'a': 0, 'as': 1, 'bat': 2, 'car': 3, 'dove': 4, 'python': 5}
```

We can also use the comprehensions with nested sequences. Imagine we have a list of lists containing some English and Spanish names. Suppose we wanted to get a single list containing all names with two or more "a"s in them. We could certainly do this with a simple for loop:

```py
all_data = [["John", "Emily", "Michael", "Mary", "Steven"], ["Maria", "Juan", "Javier", "Natalia", "Pilar"]]

for names in all_data:
  names_of_interest = [name for name in names if name.count("a") >= 2]

print(names_of_interest) # ['Maria', 'Natalia']
```

We can also wrap this whole operation up in a single nested list comprehension like this:

```py
all_data = [["John", "Emily", "Michael", "Mary", "Steven"], ["Maria", "Juan", "Javier", "Natalia", "Pilar"]]

result = [name for names in all_data for name in names if name.count("a") >= 2]

print(result)
# ['Maria', 'Natalia']
```

<hr>
<hr>

## Regex

The regular expression module `re` must be imported into your program before you can use it.

```py
import re
```

<hr>

### Using the `search` method from `re`

Here is a simple use of the `search` function from the regular expressions:

```py
import re

sentence1 = "Here is a sentence with the word text in it."
sentence2 = "Here is a sentence without the same word in it."

for sentence in [sentence1, sentence2]:
  if re.search("text", sentence):
    print(sentence)
```

Here is an example of the `search` method used on a file:

```py
import re
import os

file_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'text.txt')
textFile = open(file_path, encoding="utf-8")

for line in textFile:
  # line by line search for the 'text' in a file
  if re.search('text', line):
    print(line)
```

<hr>

### Searching the beginning of the file using the `^`

The caret character - `^` - is used in regular expressions to match the beginning of the searched text.

```py
import re

sentence1 = "Beginning of a sentence."
sentence2 = "The sentence with an ending."

for sentence in [sentence1, sentence2]:
  if re.search("^Beginning", sentence):
    print(sentence)
```

### Searching the end of the file using the `$`

When we want to match the characters at the end of the searched text, we use the `$` sign:

```py
import re

sentence1 = "Beginning of a sentence."
sentence2 = "The sentence with an ending."

for sentence in [sentence1, sentence2]:
  if re.search("ending.$", sentence):
    print(sentence)
```

<hr>

### Match any character once with `.`

The period or full stop - `.` - matches any one character.

```py
import re

sentence1 = "This is it."
sentence2 = "These are his books."

for sentence in [sentence1, sentence2]:
  if re.search(".his", sentence):
    print(sentence)
```

<hr>

### Match any character zero or more times with `*`

`*` means that the character before `*` should match zero or more times.

```py
import re

sentence1 = "This is it."
sentence2 = "These are his books."
sentence3 = "is books."
sentence4 = "  is books."

for sentence in [sentence1, sentence2, sentence3, sentence4]:
  if re.search(".*is", sentence):
    print(sentence)
```

<hr>

### Match any character once or more times with `+`

`+` means that the character before the `+` should match one or more times.

```py
import re

sentence1 = "This is it."
sentence2 = "These are his books."
sentence3 = "is books."
sentence4 = "  is books."

for sentence in [sentence1, sentence2, sentence3, sentence4]:
  if re.search(".+is", sentence):
    print(sentence)
```

<hr>

### Match any character once or zero time with `?`

`?` means that the character before the `?` should match zero or one time.

```py
import re

sentence1 = "This is it."
sentence2 = "These are his books."
sentence3 = "is books."
sentence4 = "  is books."

for sentence in [sentence1, sentence2, sentence3, sentence4]:
  if re.search(".?is", sentence):
    print(sentence)
```

<hr>

### Note about greedy mode

`*`, `+`, and `?` work in a greedy mode, meaning they are trying to match as many characters as possible. To make them work in a non-greedy mode, we use `*?`, `+?`, and `??`.

<hr>

### Using the `findall` method from `re`

`search` is not the only method that we can use for regular expressions. We can also use the `findall()` method to extract all of the substrings which match a regular expression. It provides results in a list.

```py
import re

text = 'This is the first line to be written.'

findings = re.findall('is', text)
print(findings) # ['is', 'is']
```

<hr>

### Using square brackets in Regex

In regular expressions, square brackets are used to indicate a set of multiple acceptable characters we are willing to consider matching. In the below example, `a-z` means letters from from a to z, `A-Z` means capital letters from A to Z, and `0-9` means digits from 0 to 9.

```py
import re

text = 'Here is an example email address: email@example.com.'

findings = re.findall('[a-zA-Z0-9]*@[a-zA-Z.]*', text)
print(findings) # ['email@example.com']
```

> Note that inside the square brackets, the period matches an actual period

If we use the `^` symbol in the beginning of square brackets, we invert the logic of square brackets. Normally, having characters in square brackets means one of the characters should match. But with caret, we are telling that non of the characters in the square brackets should match.

```py
import re

text = 'This is the first line to be written.'

# Don't match small letters, whitespaces, and periods
findings = re.findall('[^a-z\s.]', text)
print(findings) # ['T']
```

<hr>

### Using parentheses in Regex

**Parentheses** are another type of special characters in regular expressions. When you add parentheses to a regular expression, they are ignored when matching the string. But when you are using `findall()`, parentheses indicate that while you want the whole expression to match, you are only interested in extracting a portion of the substring that matches the regular expression.

In the below example, we match the email but only extract the website part of the match due to indicating with parentheses that we only want to extract the website part:

```py
import re

text = 'Here is an example email address: email@example.com.'

findings = re.findall('[a-zA-Z0-9]*@([a-zA-Z.]*)', text)
print(findings) # ['example.com']
```

<hr>

### Matching whitespace character with `\s` and non-whitespace character with `\S`

`\s` matches a whitespace character.

```py
import re

text = 'This is the first line to be written.'

findings = re.findall('\s+is', text)
print(findings) # [' is']
```

We can look for non-whitespace character using the `\S`.

```py
import re

text = 'This is the first line to be written.'

findings = re.findall('\S+is', text)
print(findings) # ['This']
```

<hr>

### Word boundary with `\b`

`\b` means a word boundary and it matches the empty string, but only at the start or end of a word.

```py
import re

text = ' This is the first line to be written. '

findings = re.search(r'\bis\b', text)
print(findings) # <re.Match object; span=(6, 8), match='is'>
```

Note that `\b` also means backspace in string literals. Therefore, we used the raw string in the above example. We can also escape the backspace nature of `\b` like in the below example:

```py
import re

text = ' This is the first line to be written. '

findings = re.findall('\\bis\\b', text)
print(findings) # ['is']
```

### Non-word boundary with `\B`

`\B` does the opposite of `\b`. It asserts that the regex parser’s current position must not be at the start or end of a word:

```py
import re

text = 'This is the first line to be written.'

findings = re.findall('\Bthe', text)
print(findings) # []
```

<hr>

### Match digits with `\d` and non-digits with `\D`

`\d` matches any decimal digit; equivalent to the set `[0-9]`.

```py
import re

text = 'numbers: 123,456,789'

findings = re.findall('\d', text)
print(findings) # ['1', '2', '3', '4', '5', '6', '7', '8', '9']
```

`\D` matches any non-digit character; equivalent to the set `[^0-9]`.

```py
import re

text = 'numbers: 123,456,789'

findings = re.findall('\D', text)
print(findings) # ['n', 'u', 'm', 'b', 'e', 'r', 's', ':', ' ', ',', ',']
```

<hr>

### Table of some regex methods

Regular expression methods:

| Method        | Description                                                                                                                                                                              |
| ------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `findall`     | Return all nonoverlapping matching patterns in a string as a list                                                                                                                        |
| `finditer`    | Like `findall`, but returns an iterator                                                                                                                                                  |
| `match`       | Match pattern at start of string and optionally segment pattern components into groups; if the pattern matches, return a match object, and otherwise `None`                              |
| `search`      | Scan string for match to pattern, returning a match object if so; unlike `match`, the match can be anywhere in the string as opposed to only at the beginning                            |
| `split`       | Break string into pieces at each occurrence of pattern                                                                                                                                   |
| `sub`, `subn` | Replace all (`sub`) or first n occurrences (`subn`) of pattern in string with replacement expression; use symbols \1, \2, ... to refer to match group elements in the replacement string |

<hr>
<hr>

## Python Package index and pip

Python has a rich standard library that you can use immediately in your project. In case you need a package that isn’t available in the standard library, you can find it on the Python Package Index (pypi.org).

The Python Package Index (PyPI) is the largest Python repository. It contains many Python packages developed and maintained by the Python community.

pip is the package installer for Python. Pip allows you to install packages from PyPI and other repositories.

Python comes with pip by default. To check if pip is available on your computer, you can open the command prompt (or Powershell) on Windows and type the following command:

```
pip --V
```

To install a package from PyPI, you use the following command on Windows:

```
pip install <package_name>
```

To install a package with a specific version, you use the following command:

```
pip install <package_name>==<version>
```

To list all installed packages, you use the following pip command:

```
pip list
```

To check what packages are outdated, you use the following command:

```
pip list --outdated
```

To uninstall a package, you use the pip uninstall command:

```
pip uninstall <package_name>
```

To show the dependencies of a package, you use the following command:

```
pip show <package_name>
```

To execute a shell command on a jupyter notebook, we have to use the exclamation mark - `!` - before our code:

```python
!pip install <package_name>
```

<hr>
<hr>

## Network

There is built-in support in Python called `socket` which makes it very easy to make network connections and retrieve data over those sockets in a Python program.

While we can manually send and receive data over HTTP using the `socket` library, there is a much simpler way to perform this common task in Python by using the `urllib` library. Using `urllib`, you can treat a web page much like a file. You simply indicate which web page you would like to retrieve and `urllib` handles all of the HTTP protocol and header details.

<hr>
<hr>

## Date and Time

The Python standard library includes data types for date and time data, as well as calendar-related functionality. The `datetime`, `time`, and `calendar` modules are the main places to start.

Here are some data types in the `datetime` module:

| Type        | Description                                                                       |
| ----------- | --------------------------------------------------------------------------------- |
| `datetime`  | Store both date and time                                                          |
| `timedelta` | The difference between two `datetime` values (as days, seconds, and microseconds) |
| `date`      | Store calendar date (year, month, day) using the Gregorian calendar               |
| `time`      | Store time of day as hours, minutes, seconds, and microseconds                    |
| `tzinfo`    | Base type for storing time zone information                                       |

### `now`

The `now` method retrieves the date for the current day:

```py
from datetime import datetime

now = datetime.now()
now # datetime.datetime(2024, 9, 4, 9, 43, 31, 834034)

now.year, now.month, now.day # (2024, 9, 4)
```

### `timedelta`

`datetime` stores both the date and time down to the microsecond. `datetime.timedelta`, or simply `timedelta`, represents the temporal difference between two `datetime` objects:

```py
from datetime import datetime

delta = datetime(2011, 1, 7) - datetime(2008, 6, 24, 8, 15)

delta # datetime.timedelta(days=926, seconds=56700)
delta.days # 926
delta.seconds # 56700
```

We can do arithmetic computation with `timedelta` and `datetime` objects:

```py
from datetime import timedelta

start = datetime(2011, 1, 7)

start + timedelta(12) # datetime.datetime(2011, 1, 19, 0, 0)
start - 2 * timedelta(12) # datetime.datetime(2010, 12, 14, 0, 0)
```

### Formatting `datetime` objects as strings

You can format `datetime` objects as strings using `str` or the `strftime` method, passing a format specification:

```py
stamp = datetime(2011, 1, 3)

str(stamp) # '2011-01-03 00:00:00'

stamp.strftime("%Y-%m-%d") # '2011-01-03'
```

See below table for a complete list of the format codes.

| Type | Description                                                                                                                                 |
| ---- | ------------------------------------------------------------------------------------------------------------------------------------------- |
| `%Y` | Four-digit year                                                                                                                             |
| `%y` | Two-digit year                                                                                                                              |
| `%m` | Two-digit month [01, 12]                                                                                                                    |
| `%d` | Two-digit day [01, 31]                                                                                                                      |
| `%H` | Hour (24-hour clock) [00, 23]                                                                                                               |
| `%I` | Hour (12-hour clock) [01, 12]                                                                                                               |
| `%M` | Two-digit minute [00, 59]                                                                                                                   |
| `%S` | Second [00, 61] (seconds 60, 61 account for leap seconds)                                                                                   |
| `%f` | Microsecond as an integer, zero-padded (from 000000 to 999999)                                                                              |
| `%j` | Day of the year as a zero-padded integer (from 001 to 336)                                                                                  |
| `%w` | Weekday as an integer [0 (Sunday), 6]                                                                                                       |
| `%u` | Weekday as an integer starting from 1, where 1 is Monday.                                                                                   |
| `%U` | Week number of the year [00, 53]; Sunday is considered the first day of the week, and days before the first Sunday of the year are “week 0” |
| `%W` | Week number of the year [00, 53]; Monday is considered the first day of the week, and days before the first Monday of the year are “week 0” |
| `%z` | UTC time zone offset as `+HHMM` or `-HHMM`; empty if time zone naive                                                                        |
| `%Z` | Time zone name as a string, or empty string if no time zone                                                                                 |
| `%F` | Shortcut for `%Y-%m-%d` (e.g., 2012-4-18)                                                                                                   |
| `%D` | Shortcut for `%m/%d/%y` (e.g., 04/18/12)                                                                                                    |

### Converting string dates to `datetime` objects

You can use many of the same format codes to convert strings to dates using `datetime.strptime` (but some codes, like `%F`, cannot be used):

```py
value = "2011-01-03"

datetime.strptime(value, "%Y-%m-%d") # datetime.datetime(2011, 1, 3, 0, 0)

datestrs = ["7/6/2011", "8/6/2011"]

[datetime.strptime(x, "%m/%d/%Y") for x in datestrs]
# [datetime.datetime(2011, 7, 6, 0, 0), datetime.datetime(2011, 8, 6, 0, 0)]
```

### Locale-specific date formatting

`datetime` objects also have a number of locale-specific formatting options for systems in other countries or languages.

| Type | Description                                                                                     |
| ---- | ----------------------------------------------------------------------------------------------- |
| `%a` | Abbreviated weekday name                                                                        |
| `%A` | Full weekday name                                                                               |
| `%b` | Abbreviated month name                                                                          |
| `%B` | Full month name                                                                                 |
| `%c` | Full date and time (e.g., ‘Tue 01 May 2012 04:20:57 PM’)                                        |
| `%p` | Locale equivalent of AM or PM                                                                   |
| `%x` | Locale-appropriate formatted date (e.g., in the United States, May 1, 2012 yields ‘05/01/2012’) |
| `%X` | Locale-appropriate time (e.g., ‘04:24:12 PM’)                                                   |
