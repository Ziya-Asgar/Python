# Modules

In Python, a module is simply a file with the `.py` extension containing Python code. Let's say we have a file named `module.py` with the below code:

```py
# module.py
simpleString = "simple string"

def func(arg):
  print(arg)
```

We can import and use the `module.py` in the `test.py`, located in the same directory, this way:

```py
# test.py
import module

print(module.simpleString) # simple string
module.func('running module.func from test.py') # running module.func from test.py
```

By using the `as` keyword, you can give imports different variable names:

```py
import module as md
# from module import simpleString, func

print(md.simpleString) # simple string
md.func('running module.func from test.py') # running module.func from test.py
```

We can also import specific variables:

```py
# test.py
from module import simpleString, func

print(simpleString) # simple string
func('running module.func from test.py') # running module.func from test.py
```

The command `from <module_name> import *` imports all variables and functions from `<module_name>` into the current workspace. However, use of this syntax is discouraged! It clutters up the current workspace, and one risks overwriting existing variables with the same name as an imported variable.

---

---
