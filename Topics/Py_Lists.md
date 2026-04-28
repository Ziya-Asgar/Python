# Lists

- [Lists](#lists)
  - [Creating a list](#creating-a-list)
  - [Accessing list items](#accessing-list-items)
  - [Using the `in` operator with lists](#using-the-in-operator-with-lists)
  - [Looping through lists with the `for` loop](#looping-through-lists-with-the-for-loop)
  - [Using `+` and `*` operators with lists](#using--and--operators-with-lists)
  - [List Methods](#list-methods)
    - [`append`](#append)
    - [`extend`](#extend)
    - [`insert`](#insert)
    - [`sort`](#sort)
    - [The `sorted` function](#the-sorted-function)
    - [`reverse`](#reverse)
  - [Deleting List Elements](#deleting-list-elements)

---

---

Like a string, a list is a sequence of values. In a string, the values are characters; in a list, they can be any type. The values in lists are called elements or sometimes items.

---

---

## Creating a list

There are several ways to create a new list; the simplest is to enclose the elements in square brackets (“[” and ”]”):

```py
# list of integers
[10, 20, 30, 40]

# list of strings
['item 1', 'item 2', 'item 3']

# list of different data types
['some list item', 2.0, 5, [10, 20]]

# a list assigned to a variable
listVariable = ['item 1']
```

Another way to create a list item is to use the `list` function. If no argument is provided, it creates an empty list. If the argument is provided, the argument should be an iterable object, like a tuple or string:

```py
print(list()) # []

listVar = list("text")

print(listVar) # ['t', 'e', 'x', 't']
```

## Accessing list items

We can access the list items using the square bracket notation:

```py
listVariable = [1, 2, 3, 4]

print(listVariable[0]) # 1
print(listVariable[1:3]) # [2, 3]
print(listVariable[:]) # [1, 2, 3, 4]
```

If an index provided to the bracket notation has a negative value, it counts backward from the end of the list.

```py
listVariable = [1, 2, 3, 4]

print(listVariable[-1]) # 4
print(listVariable[-2]) # 3
```

We have so far used the slicing notation with `[start:stop]`. We can also use the third item, which is step, with the slice notation, to indicate which elements should be accessed:

```py
listVariable = [1, 2, 3, 4, 5, 6, 7, 8, 9]

# every second element from index 1 to 8
print(listVariable[1:8:2]) # [2, 4, 6, 8]

# every third element from index 1 to the end of the list
print(listVariable[1::3]) # [2, 5, 8]
```

A clever use of this is to pass -1, which has the useful effect of reversing a list.

```py
listVariable = [1, 2, 3, 4, 5, 6, 7, 8, 9]

print(listVariable[::-1]) # [9, 8, 7, 6, 5, 4, 3, 2, 1]
```

We can also assign items to a specific position in a list using the bracket notation:

```py
listVariable = [1, 2, 3, 4]

print(listVariable[0]) # 1

listVariable[0] = 5
print(listVariable[0]) # 5

listVariable[1:3] = [6, 7]
print(listVariable) # [5, 6, 7, 4]
```

---

---

## Using the `in` operator with lists

The `in` operator also works on lists.

```py
listVariable = ['item 1', 'item 2', 'item 3']

print('item 1' in listVariable) # True
print('item 4' in listVariable) # False
```

The keyword `not` can be used to negate `in`:

```py
listVariable = ['item 1', 'item 2', 'item 3']

print('item 1' not in listVariable) # False
print('item 4' not in listVariable) # True
```

---

---

## Looping through lists with the `for` loop

To traverse the list, we can use the `for` loop. However, to update the items in a list, we need indices as well. To have both indices and traverse the list, we can use the `range` function:

```py
numbers = [1, 2, 3, 4]

for i in range(len(numbers)):
  numbers[i] = numbers[i] ** 2

print(numbers) # [1, 4, 9, 16]
```

A `for` loop over an empty list never executes the body:

```py
empty = []

for x in empty:
  print('This never happens.')
```

---

---

## Using `+` and `*` operators with lists

The `+` operator used on two and more lists, concatenates those lists:

```py
a = [1, 2, 3]
b = [4, 5, 6]
c = a + b

print(c)
# [1, 2, 3, 4, 5, 6]
```

We can also use the `+` operator to add to an existing list:

```py
listVar = [1, 2, 3]
listVar = listVar + [4]

print(listVar) # [1, 2, 3, 4]
```

The `*` operator repeats a list a given number of times:

```py
print([0] * 4)
# [0, 0, 0, 0]

print([1, 2, 3] * 3)
# [1, 2, 3, 1, 2, 3, 1, 2, 3]
```

---

---

## List Methods

Most list methods are void; they modify the list and return `None`.

---

### `append`

The `append` method adds a new element to the end of a list:

```py
listVar = ['a', 'b', 'c']
listVar.append('d')

print(listVar) # ['a', 'b', 'c', 'd']
```

---

### `extend`

The `extend` method takes a list as an argument and appends all of the elements:

```py
listVar1 = ["a", "b", "c"]
listVar2 = ["d", "e"]
listVar1.extend(listVar2)

print(listVar1) # ['a', 'b', 'c', 'd', 'e']
```

---

### `insert`

Using `insert` you can insert an element at a specific location in the list:

```py
listVar = [1, 2, 3, 4]
listVar.insert(2, 'three')

print(listVar) # [1, 2, 'three', 3, 4]
```

---

### `sort`

The `sort` method arranges the elements of the list from low to high:

```py
listVar = ['d', 'c', 'e', 'b', 'a']
listVar.sort()

print(listVar) # ['a', 'b', 'c', 'd', 'e']
```

To sort in the reverse order, we can use `.sort(reverse=True)`:

```py
listVar = ['d', 'c', 'e', 'b', 'a']
listVar.sort(reverse=True)

print(listVar) # ['e', 'd', 'c', 'b', 'a']
```

`sort` has a few options that will occasionally come in handy. One is the ability to pass a secondary sort key—that is, a function that produces a value to use to sort the objects.

```py
listVar = ["saw", "small", "He", "foxes", "six"]
listVar.sort(key=len)

print(listVar)
```

---

### The `sorted` function

The `sorted` function returns a new sorted list from the elements of any sequence. It doesn't modify the original list:

```py
listVar = ['d', 'c', 'e', 'b', 'a']
newList = sorted(listVar)

print(listVar) # ['d', 'c', 'e', 'b', 'a']
print(newList) # ['a', 'b', 'c', 'd', 'e']
```

Unlike the `sort` method, the `sorted` function also works on strings.

```py
stringVar = 'hello'

print(sorted(stringVar)) # ['e', 'h', 'l', 'l', 'o']
```

---

### `reverse`

The `reverse` method reverses the list in place:

```py
listVar = [1, 2, 3, 4]
listVar.reverse()

print(listVar) # [4, 3, 2, 1]
```

---

---

## Deleting List Elements

If you know the index of the element you want to delete, you can use the `pop` method. `pop` modifies the list and returns the element that was removed. If you don’t provide an index, it deletes and returns the last element:

```py
listVar = ['a', 'b', 'c']
deletedItem = listVar.pop(1)

print(listVar) # ['a', 'c']
print(deletedItem) # b

lastItem = listVar.pop()

print(listVar) # ['a']
print(lastItem) # c
```

If you don’t need the removed value, you can use the `del` statement:

```py
listVar = ['a', 'b', 'c']

del listVar[1]

print(listVar) # ['a', 'c']
```

To remove more than one element, you can use `del` with slice indexing:

```py
listVar = ['a', 'b', 'c', 'd', 'e', 'f']

del listVar[1:5]

print(listVar) # ['a', 'f']
```

If you know the element you want to remove (but not the index), you can use the `remove` method. The return value from `remove` is `None`:

```py
listVar = ['a', 'b', 'c', 'd', 'e', 'f']

listVar.remove('c')

print(listVar) # ['a', 'b', 'd', 'e', 'f']
```

---

---
