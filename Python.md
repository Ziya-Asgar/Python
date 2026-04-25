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
    - [`count`](#count)
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
  - [External Python packages](#external-python-packages)
    - [`pip`](#pip)
    - [`uv`](#uv)
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

## External Python packages

Python has a rich standard library that you can use immediately in your project. In case you need a package that isn’t available in the standard library, you can find it on the Python Package Index (pypi.org).

The Python Package Index (PyPI) is the largest Python repository. It contains many Python packages developed and maintained by the Python community.

### `pip`

Pip is the package installer for Python. Pip allows you to install packages from PyPI and other repositories.

Python comes with `pip` by default. To check if pip is available on your computer, you can open the command prompt (or Powershell) on Windows and type the following command:

```
pip --version
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

### `uv`

`uv` is a fast Python package and project manager. There are different ways to install `uv`. However, considering that python comes with `pip`, one easy way to install `uv` is to use the below command:

```sh
pip install uv
```

To run a python code (in a `.py` file) with `uv`, we can use the below code:

```sh
uv run file_name.py
```

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
