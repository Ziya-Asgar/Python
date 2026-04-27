# List, Set, and Dictionary Comprehensions

List comprehensions allow you to concisely form a new list by filtering the elements of a collection, transforming the elements passing the filter into one concise expression. The filter condition can be omitted, leaving only the expression. List comprehension takes the basic form:

```py
[expr for value in collection if condition]
```

For example, given a list of strings, we could filter out strings with length 2 or less and convert them to uppercase like this:

```py
strings = ["a", "as", "bat", "car", "dove", "python"]

newList = [x.upper() for x in strings if len(x) > 2]
print(newList) # ['BAT', 'CAR', 'DOVE', 'PYTHON']
```

We can also change the position of the `if` and add `else` to it:

```py
strings = ["a", "as", "bat", "car", "dove", "python"]

newList = [x.upper() if len(x) > 2 else 0 for x in strings]
print(newList) # [0, 0, 'BAT', 'CAR', 'DOVE', 'PYTHON']
```

---

A set comprehension looks like the equivalent list comprehension except with curly braces instead of square brackets:

```py
set_comp = {expr for value in collection if condition}
```

Here is an example:

```py
strings = ["a", "as", "bat", "car", "dove", "python"]

unique_lengths = {len(x) for x in strings}
print(unique_lengths) # {1, 2, 3, 4, 6}
```

---

A dictionary comprehension looks like this:

```py
dict_comp = {key: value for value in collection if condition}
```

Here is an example:

```py
strings = ["a", "as", "bat", "car", "dove", "python"]

newDictionary = {value: index for index, value in enumerate(strings)}
print(newDictionary) # {'a': 0, 'as': 1, 'bat': 2, 'car': 3, 'dove': 4, 'python': 5}
```

We can also use the comprehensions with nested sequences. Imagine we have a list of lists containing some English and Spanish names. Suppose we wanted to get a single list containing all names with two or more "a"s in them. We could certainly do this with a simple for loop:

```py
all_data = [["John", "Emily", "Michael", "Mary", "Steven"], ["Maria", "Juan", "Javier", "Natalia", "Pilar"]]

for names in all_data:
  names_of_interest = [name for name in names if name.count("a") >= 2]

print(names_of_interest) # ['Maria', 'Natalia']
```

We can also wrap this whole operation up in a single nested list comprehension like this:

```py
all_data = [["John", "Emily", "Michael", "Mary", "Steven"], ["Maria", "Juan", "Javier", "Natalia", "Pilar"]]

result = [name for names in all_data for name in names if name.count("a") >= 2]

print(result)
# ['Maria', 'Natalia']
```

---

---
