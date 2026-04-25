# Dictionaries

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

---

---

A dictionary is like a list, but more general. In a list, the index positions have to be integers; in a dictionary, the indices can be (almost) any type. You can think of dictionaries as the mapping between keys and values.

---

---

## Creating a dictionary

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

---

---

## Accessing dictionary items

We use the keys to look up the corresponding values in a dictionary:

```py
eng2sp = {'one': 'uno', 'two': 'dos', 'three': 'tres'}

print(eng2sp['two']) # 'dos'
```

---

---

## Adding dictionary items

Here is how add items to a dictionary, after creating it:

```py
eng2sp = dict()

eng2sp['one'] = 'uno'

print(eng2sp) # {'one': 'uno'}
```

---

---

## Using `len` function on dictionaries

The `len` function works on dictionaries; it returns the number of key-value pairs:

```py
eng2sp = {'one': 'uno', 'two': 'dos', 'three': 'tres'}

print(len(eng2sp)) # 3
```

---

---

## Using `in` operator with dictionaries

The `in` operator works on dictionaries; it tells you whether something appears as a key in the dictionary:

```py
eng2sp = {'one': 'uno', 'two': 'dos', 'three': 'tres'}

print('one' in eng2sp) # True
print('uno' in eng2sp) # False
```

---

---

## The `values` method

To get all the values in a dictionary, we can use the `values` method:

```py
eng2sp = {'one': 'uno', 'two': 'dos', 'three': 'tres'}

vals = list(eng2sp.values())
print(vals) # ['uno', 'dos', 'tres']

print('uno' in vals) # True
```

---

---

## The `keys` method

In addition to `values` method, there is also `keys` method available in dictionary objects:

```py
eng2sp = {'one': 'uno', 'two': 'dos', 'three': 'tres'}

keysInDictionary = list(eng2sp.keys())
print(keysInDictionary) # ['one', 'two', 'three']
```

---

---

## The `items` method

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

---

---

## `get`

Dictionaries have a method called `get` that takes a key and a default value. If the key appears in the dictionary, `get` returns the corresponding value; otherwise it returns the default value.

```py
dictionary = {'one': 1, 'two': 2, 'three': 3}

print(dictionary.get('one', 1)) # 1
print(dictionary.get('two', 10)) # 2
print(dictionary.get('four', 4)) # 4
```

---

---

## `update`

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

---

---

## Looping through dictionary items

To loop through the dictionary, we can use the `for` loop:

```py
dictionary = {'one': 1, 'two': 2, 'three': 3}

for key in dictionary:
  print(key, dictionary[key])
```

---

---

## Deleting items from a dictionary

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

---

---

## Dictionary unpacking with `**`

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

---

---
