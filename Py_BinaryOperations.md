# Binary operations

Most of the binary math operations and comparisons use familiar mathematical syntax in Python.

- Add a and b with `+`

```py
a = 1
b = 2

print(a + b) # 3
```

- Subtract b from a with `-`

```py
a = 1
b = 2

print(a - b) # -1
```

- Multiply a by b with `*`

```py
a = 1
b = 2

print(a * b) # 2
```

- Divide a by b with `/`

```py
a = 1
b = 2

print(a / b) # 0.5
```

- Floor-divide a by b with `//`, dropping any fractional remainder. Using this always returns an integer:

```py
a = 1
b = 2

print(a // b) # 0
```

- Raise a to the b power with `**`

```py
a = 5
b = 2

exponentiation = a ** b

print(exponentiation) # 25
```

The modulus operator works on integers and yields the remainder of the division. In Python, the modulus operator is a percent sign (`%`).

```py
remainder = 7 % 3

print(remainder) # 1
```

---

`+` and `*` are an addition and a multiplication operators. But they are also used for string concatenation:

```py
strNum1 = '100'
strNum2 = '150'

print(strNum1 + strNum2) # 100150
```

```py
strNum1 = 'Test '
strNum2 = 3

print(strNum1 * strNum2) # Test Test Test
```

---

---
