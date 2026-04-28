# Generators

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

---

---
