# Python

- [Python](#python)
  - [Some Useful Links](#some-useful-links)
  - [Intro](#intro)
  - [Modules](#modules)
  - [Variables](#variables)
  - [Strings](#strings)
  - [Binary Operations](#binary-operations)
  - [User Input](#user-input)
  - [Type Conversion](#type-conversion)
  - [Conditionals](#conditionals)
  - [Error Handling](#error-handling)
  - [Functions](#functions)
  - [Generators](#generators)
  - [Loops](#loops)
  - [Working With Files](#working-with-files)
  - [Lists](#lists)
  - [Dictionaries](#dictionaries)
  - [Tuples](#tuples)
  - [Iterable Unpacking](#iterable-unpacking)
  - [Classes](#classes)
  - [Sets](#sets)
  - [List, Set, and Dictionary Comprehensions](#list-set-and-dictionary-comprehensions)
  - [External Modules](#external-modules)
  - [Virtual Environments](#virtual-environments)
    - [Creating a virtual environment](#creating-a-virtual-environment)
    - [Activating and deactivating a virtual environment](#activating-and-deactivating-a-virtual-environment)
    - [requirements.txt file](#requirementstxt-file)
  - [Built-in Modules](#built-in-modules)
    - [Date and Time](#date-and-time)
      - [`now`](#now)
      - [`timedelta`](#timedelta)
      - [Formatting `datetime` objects as strings](#formatting-datetime-objects-as-strings)
      - [Converting string dates to `datetime` objects](#converting-string-dates-to-datetime-objects)
      - [Locale-specific date formatting](#locale-specific-date-formatting)
    - [`random` module](#random-module)
    - [`math` module](#math-module)
    - [`os` module](#os-module)
      - [`getcwd()`](#getcwd)
      - [`listdir()`](#listdir)
      - [`makedirs()`](#makedirs)
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
    - [Network](#network)

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

[Intro](./Py_Intro.md)

<hr>
<hr>

## Modules

[Modules](./Py_Modules.md)

<hr>
<hr>

## Variables

[Variables](./Py_Variables.md)

<hr>
<hr>

## Strings

[Strings](./Py_Strings.md)

<hr>
<hr>

## Binary Operations

[Binary Operations](./Py_BinaryOperations.md)

<hr>
<hr>

## User Input

[User Input](./Py_UserInput.md)

<hr>
<hr>

## Type Conversion

[Type Conversion](./Py_TypeConversion.md)

<hr>
<hr>

## Conditionals

[Conditionals](./Py_Conditionals.md)

<hr>
<hr>

## Error Handling

[Error Handling](./Py_ErrorHandling.md)

<hr>
<hr>

## Functions

[Functions](./Py_Functions.md)

<hr>
<hr>

## Generators

[Generators](./Py_Generators.md)

<hr>
<hr>

## Loops

[Loops](./Py_Loops.md)

<hr>
<hr>

## Working With Files

[Working With Files](./Py_WorkingWithFiles.md)

<hr>
<hr>

## Lists

[Lists](./Py_Lists.md)

<hr>
<hr>

## Dictionaries

[Dictionaries](./Py_Dictionaries.md)

<hr>
<hr>

## Tuples

[Tuples](./Py_Tuples.md)

<hr>
<hr>

## Iterable Unpacking

[Iterable Unpacking](./Py_IterableUnpacking.md)

<hr>
<hr>

## Classes

[Classes](./Py_Classes.md)

<hr>
<hr>

## Sets

[Sets](./Py_Sets.md)

<hr>
<hr>

## List, Set, and Dictionary Comprehensions

[List, Set, and Dictionary Comprehensions](./Py_List_Set_Dictionary_Comprehensions.md)

<hr>
<hr>

## External Modules

[External Modules](./Py_ExternalModules.md)

<hr>
<hr>

## Virtual Environments

A virtual environment is a self-contained location that enables to maintain a separate and isolated environments for python projects. It helps to manage dependencies, versions, and packages without conflicts accross different projects.

A virtual environment is also a separate directory. So, when we create one, it is recommended to be in folder where a specific python project is.

<hr>

### Creating a virtual environment

This is how we can create one on a windows machine:

```sh
python -m venv env_name
```

<hr>

### Activating and deactivating a virtual environment

After this command, a directory named **env_name** will be created. To activate the environment, we need to run the code below on windows:

```sh
source env_name/Scripts/activate
```

If the above doesn't work, we can try:

```sh
source env_name/Scripts/activate.bat
```

To deactivate, we run `deactivate`.

<hr>

### requirements.txt file

To share the project with others, it's recommended to create a file named `requirements.txt` and the save dependencies to that file. This way we can avoid pushing the whole environment to Git. To create the `requirements.txt` file with all the dependencies, we can use the below code:

```sh
pip freeze > requirements.txt
```

`pip freeze` is a shell command to list all the python libraries and versions. `>` is an operator that pipes the output of `pip freeeze` to the `requirements.txt` file.

After this step, another person can activate a different environment on their end and use this `requirements.txt` file to install all the dependencies. The code that is needed is below:

```sh
pip install -r requirements.txt
```

`-r` stands for installing from a file.

<hr>
<hr>

## Built-in Modules

### Date and Time

The Python standard library includes data types for date and time data, as well as calendar-related functionality. The `datetime`, `time`, and `calendar` modules are the main places to start.

Here are some data types in the `datetime` module:

| Type        | Description                                                                       |
| ----------- | --------------------------------------------------------------------------------- |
| `datetime`  | Store both date and time                                                          |
| `timedelta` | The difference between two `datetime` values (as days, seconds, and microseconds) |
| `date`      | Store calendar date (year, month, day) using the Gregorian calendar               |
| `time`      | Store time of day as hours, minutes, seconds, and microseconds                    |
| `tzinfo`    | Base type for storing time zone information                                       |

#### `now`

The `now` method retrieves the date for the current day:

```py
from datetime import datetime

now = datetime.now()
now # datetime.datetime(2024, 9, 4, 9, 43, 31, 834034)

now.year, now.month, now.day # (2024, 9, 4)
```

#### `timedelta`

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

#### Formatting `datetime` objects as strings

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

#### Converting string dates to `datetime` objects

You can use many of the same format codes to convert strings to dates using `datetime.strptime` (but some codes, like `%F`, cannot be used):

```py
value = "2011-01-03"

datetime.strptime(value, "%Y-%m-%d") # datetime.datetime(2011, 1, 3, 0, 0)

datestrs = ["7/6/2011", "8/6/2011"]

[datetime.strptime(x, "%m/%d/%Y") for x in datestrs]
# [datetime.datetime(2011, 7, 6, 0, 0), datetime.datetime(2011, 8, 6, 0, 0)]
```

#### Locale-specific date formatting

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

---

### `random` module

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

### `math` module

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

### `os` module

We can use various methods provided in the `os` module to get the information about the operating system. Before we can use the module, we have to import it:

```py
import os
```

<hr>

#### `getcwd()`

The `getcwd()` method provides the link of the current working directory (where the python runs):

```py
import os

print(os.getcwd())
```

<hr>

#### `listdir()`

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

#### `makedirs()`

The `makedirs()` method creates a new directory. If `exist_ok=True`, then it won't throw an exception when the folder already exists and it won't override the existing folder:

```py
import os

os.makedirs("./newFolder", exist_ok=True)
```

<hr>

### Regex

The regular expression module `re` must be imported into your program before you can use it.

```py
import re
```

<hr>

#### Using the `search` method from `re`

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

#### Searching the beginning of the file using the `^`

The caret character - `^` - is used in regular expressions to match the beginning of the searched text.

```py
import re

sentence1 = "Beginning of a sentence."
sentence2 = "The sentence with an ending."

for sentence in [sentence1, sentence2]:
  if re.search("^Beginning", sentence):
    print(sentence)
```

#### Searching the end of the file using the `$`

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

#### Match any character once with `.`

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

#### Match any character zero or more times with `*`

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

#### Match any character once or more times with `+`

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

#### Match any character once or zero time with `?`

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

#### Note about greedy mode

`*`, `+`, and `?` work in a greedy mode, meaning they are trying to match as many characters as possible. To make them work in a non-greedy mode, we use `*?`, `+?`, and `??`.

<hr>

#### Using the `findall` method from `re`

`search` is not the only method that we can use for regular expressions. We can also use the `findall()` method to extract all of the substrings which match a regular expression. It provides results in a list.

```py
import re

text = 'This is the first line to be written.'

findings = re.findall('is', text)
print(findings) # ['is', 'is']
```

<hr>

#### Using square brackets in Regex

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

#### Using parentheses in Regex

**Parentheses** are another type of special characters in regular expressions. When you add parentheses to a regular expression, they are ignored when matching the string. But when you are using `findall()`, parentheses indicate that while you want the whole expression to match, you are only interested in extracting a portion of the substring that matches the regular expression.

In the below example, we match the email but only extract the website part of the match due to indicating with parentheses that we only want to extract the website part:

```py
import re

text = 'Here is an example email address: email@example.com.'

findings = re.findall('[a-zA-Z0-9]*@([a-zA-Z.]*)', text)
print(findings) # ['example.com']
```

<hr>

#### Matching whitespace character with `\s` and non-whitespace character with `\S`

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

#### Word boundary with `\b`

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

#### Non-word boundary with `\B`

`\B` does the opposite of `\b`. It asserts that the regex parser’s current position must not be at the start or end of a word:

```py
import re

text = 'This is the first line to be written.'

findings = re.findall('\Bthe', text)
print(findings) # []
```

<hr>

#### Match digits with `\d` and non-digits with `\D`

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

#### Table of some regex methods

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

### Network

There is built-in support in Python called `socket` which makes it very easy to make network connections and retrieve data over those sockets in a Python program.

While we can manually send and receive data over HTTP using the `socket` library, there is a much simpler way to perform this common task in Python by using the `urllib` library. Using `urllib`, you can treat a web page much like a file. You simply indicate which web page you would like to retrieve and `urllib` handles all of the HTTP protocol and header details.

<hr>
<hr>
