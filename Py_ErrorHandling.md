# Error Handling

- [Error Handling](#error-handling)
  - [`try` / `except`](#try--except)
  - [`exit`](#exit)
  - [Specifying the Type of Error](#specifying-the-type-of-error)
  - [`finally` clause](#finally-clause)
  - [`else` in `try` / `except`](#else-in-try--except)
  - [`raise`](#raise)

---

---

## `try` / `except`

There is a conditional execution structure built into Python to handle expected and unexpected errors called `try` / `except`. The `except` block is ignored if there is no error.

```py
numInp = input("Please provide a number\n")

try:
  integer = int(numInp)
  print(f"Your integer is {integer}")
except:
  print("You didn't provide a number")
```

---

---

## `exit`

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

---

---

## Specifying the Type of Error

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

---

---

## `finally` clause

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

---

---

## `else` in `try` / `except`

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

---

---

## `raise`

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

---

---
