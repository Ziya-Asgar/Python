# Iterable Unpacking

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

---

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

---

---
