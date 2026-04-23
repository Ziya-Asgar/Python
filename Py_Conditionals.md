# Conditionals

- [Conditionals](#conditionals)
  - [Comparison Operators](#comparison-operators)
  - [Logical Operators](#logical-operators)
  - [`if` statement](#if-statement)

---

---

## Comparison Operators

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

---

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

---

---

## Logical Operators

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

---

---

## `if` statement

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

---

---
