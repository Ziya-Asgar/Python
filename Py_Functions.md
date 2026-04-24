# Functions

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

---

---

## Creating a Function

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

---

### `return`

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

---

### Positional and Keyword arguments

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

---

### Assigning variables outside of a function with `global`

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

---

---

## Lambda functions

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

---

---

## `*args` and `**kwargs`

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

---

---

## Decorators

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

---

---

## Some Built-in Functions

### `max` and `min`

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

---

### `len`

`len` function tells us the length of its argument:

```py
# sequence of characters
print(len("Hello World")) # 11

# a tuple
print(len((1, 2, 3))) # 3

# a list
print(len([1, 2, 3])) # 3
```

---

### `sum`

The `sum` function returns the sum of the sequence provided to it:

```py
# a tuple
print(sum((1, 2, 3))) # 6

# a list
print(sum([1, 2, 3])) # 6
```

The `sum()` function only works when the sequence elements are numbers. The other functions (`max()`, `len()`, etc.) work with sequence of strings and other types that can be comparable.

---

### `dir`

Python has a function called `dir` which lists the attributes available for an object.

```py
text = "some text"

print(dir(text))
print(dir(int))
```

---

### `help`

You can use `help` to get some simple documentation on a method:

```py
print(help(dir))
```

---

### `range`

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

---

### `enumerate`

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

---

### `zip`

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

---

### `reversed`

`reversed` iterates over the elements of a sequence in reverse order. Keep in mind that `reversed` is a generator, so it does not create the reversed sequence until materialized (e.g., with `list` or a `for` loop):

```py
seq1 = [1, 2, 3]

print(list(seq1)) # [1, 2, 3]
```

---

### `map`

The `map` function takes a function and a sequence, and applies that function on every item of the sequence:

```py
listVar = ['one', 'two', 'three']

newList = list(map(str.capitalize, listVar))

print(newList) # ['One', 'Two', 'Three']
```

---

### `filter`

The `filter` built-in function takes a function and an iterable as arguments. It applies the function to each item in the iterable and returns a new iterable containing only the items for which the function returns `True`.

```py
def is_even(x):
    return x % 2 == 0

numbers = [1, 2, 3, 4, 5, 6]

even_numbers = list(filter(is_even, numbers))

print(even_numbers)  # [2, 4, 6]
```

---

---
