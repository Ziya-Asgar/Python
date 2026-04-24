# Loops

- [Loops](#loops)
  - [`while` loop](#while-loop)
  - [`for` loop](#for-loop)
  - [`break` statement](#break-statement)
  - [`continue` statement](#continue-statement)

---

---

## `while` loop

Here is how to define a `while` loop in Python:

```py
n = 5
while n > 0:
  print(n)
  n = n - 1

print("Loop ended")
```

Instead of incrementing `n` using `n = n - 1`, `n = n + 1`, we can use `n -= 1`, `n += 1`, etc.

---

---

## `for` loop

`for` loops are for iterating over a collection (like a list or tuple) or an iterater.

Here is an example of a `for` loop:

```py
listVar = ["item 1", "item 2", "item 3"]

for item in listVar:
  print(item)

print("Done")
"""
item 1
item 2
item 3
Done
"""
```

In the same manner, we can loop through a string:

```py
for char in "word":
  print(char)
```

---

---

## `break` statement

To manually break the loop, we use the `break` statement:

```py
n = 5
while n > 0:
  print(n)
  n = n - 1
  if (n == 3):
    break

print("Loop ended")
"""
5
4
Loop ended
"""
```

The `break` keyword only terminates the innermost loop; any outer loops will continue to run:

```py
for outer in range(3):
  for inner in range(3):
    if inner > outer:
      print("")
      break
    print(f"outer: {outer}, inner: {inner}")
"""
outer: 0, inner: 0

outer: 1, inner: 0
outer: 1, inner: 1

outer: 2, inner: 0
outer: 2, inner: 1
outer: 2, inner: 2
"""
```

---

---

## `continue` statement

You can use the `continue` statement to skip to the next iteration without finishing the body of the loop for the current iteration:

```py
n = 4
while n > 0:
  n -= 1
  if (n == 2):
    continue
  print(n)

print("Loop ended")
"""
3
1
0
Loop ended
"""
```

---

---
