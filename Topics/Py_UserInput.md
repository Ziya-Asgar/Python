# User Input

Sometimes we would like to take the value for a variable from a user. Python provides a built-in function called `input` that gets input from the keyboard. When this function is called, the program stops and waits for the user to type something. When the user presses Return or Enter, the program resumes and `input` returns what the user typed as a string.

```py
inp = input()
# user types "testing"

print(inp)
# testing
```

You can pass a string to the `input` function to be displayed to the user while asking for an input:

```py
name = input("What is your name?\n")

print(f"Hello, {name}")
```

---

---
