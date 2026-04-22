# Variables

An important characteristic of the Python language is the consistency of its object model. Every number, string, data structure, function, class, module, and so on exists in the Python interpreter in its own “box,” which is referred to as a Python object. Each object has an associated type (e.g., integer, string, or function) and internal data.

---

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

---

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

---

We can assign the same value to multiple variables at once:

```py
var1 = var2 = var3 = "some variable"

print(var1) # some variable
print(var2) # some variable
print(var3) # some variable
```

---

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

---

---
