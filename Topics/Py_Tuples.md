# Tuples

- [Tuples](#tuples)
  - [Creating a tuple](#creating-a-tuple)
  - [Accessing tuple elements](#accessing-tuple-elements)
  - [Some possible modifications in a tuple](#some-possible-modifications-in-a-tuple)
  - [Using `+` and `*` operators with tuples](#using--and--operators-with-tuples)
  - [`count`](#count)

---

---

Syntactically, a tuple is a comma-separated list of values. The values stored in a tuple can be any type, and they are indexed by integers. The important difference is that tuples are **immutable**. Tuples are also comparable and hashable so we can sort lists of them and use tuples as key values in Python dictionaries.

---

---

## Creating a tuple

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

---

---

## Accessing tuple elements

We can access the elements in a tuple using the square bracket syntax:

```py
t = ('a', 'b', 'c', 'd', 'e')

print(t[0]) # 'a'
print(t[1:3]) # ('b', 'c')
```

---

---

## Some possible modifications in a tuple

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

---

---

## Using `+` and `*` operators with tuples

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

---

---

## `count`

The `count` method, counts the number of occurrences of a value in a tuple:

```py
t = (1, 2, 2, 2, 3, 4, 2)

t.count(2) # 4

# `count` also works on strings and lists
"hello".count("l") # 2
[1, 2, 2, 2, 3, 4, 2].count(2) # 2
```

---

---
