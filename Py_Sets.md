# Sets

- [Sets](#sets)
  - [Creating sets](#creating-sets)
  - [Mathematical operations on sets](#mathematical-operations-on-sets)
    - [Union](#union)
    - [Intersection](#intersection)
    - [Difference](#difference)
    - [Symmetric difference](#symmetric-difference)
  - [`issubset`](#issubset)
  - [`issuperset`](#issuperset)
  - [`isdisjoint`](#isdisjoint)
  - [`add`](#add)
  - [`clear`](#clear)
  - [Deleting set elements](#deleting-set-elements)
  - [Equality of sets](#equality-of-sets)

---

---

A set is an unordered collection of unique elements.

Like dictionary keys, set elements generally must be immutable, and they must be hashable (which means that calling `hash` on a value does not raise an exception). In order to store list-like elements (or other mutable sequences) in a set, you can convert them to tuples.

---

---

## Creating sets

A set can be created in two ways: via the `set` function or via a set literal with curly braces:

```py
mySet1 = set([2, 2, 2, 1, 3, 3])
mySet2 = {2, 2, 2, 1, 3, 3}

print(mySet1) # {1, 2, 3}
print(mySet2) # {1, 2, 3}
```

---

---

## Mathematical operations on sets

Sets support mathematical set operations like union, intersection, difference, and symmetric difference. If you pass an input that is not a set to methods like `union` and `intersection`, Python will convert the input to a set before executing the operation. When using the binary operators, both objects must already be sets.

---

### Union

The union of the two sets is the set of distinct elements occurring in either set. This can be computed with either the `union` method or the `|` binary operator:

```py
a = {1, 2, 3, 4, 5}
b = {3, 4, 5, 6, 7, 8}

c = a.union(b)
print(c) # {1, 2, 3, 4, 5, 6, 7, 8}

c = a | b
print(c) # {1, 2, 3, 4, 5, 6, 7, 8}
```

The above methods don't change the original sets. However, we can change the set to the union, using the `update` method or `|=` operator:

```py
a = {1, 2, 3, 4, 5}
b = {3, 4, 5, 6, 7, 8}

a.update(b)

print(a) # {1, 2, 3, 4, 5, 6, 7, 8}
```

```py
a = {1, 2, 3, 4, 5}
b = {3, 4, 5, 6, 7, 8}

a |= b

print(a) # {1, 2, 3, 4, 5, 6, 7, 8}
```

---

### Intersection

The intersection contains the elements occurring in both sets. This can be computed with either the `intersection` method or `&` operator:

```py
a = {1, 2, 3, 4, 5}
b = {3, 4, 5, 6, 7, 8}

c = a.intersection(b)
print(c) # {3, 4, 5}

c = a & b
print(c) # {3, 4, 5}
```

The intersection method and operator do not change the original sets. To update the original set, we can use the `intersection_update` method or `&=` operator:

```py
a = {1, 2, 3, 4, 5}
b = {3, 4, 5, 6, 7, 8}

a.intersection_update(b)

print(a) # {3, 4, 5}
```

```py
a = {1, 2, 3, 4, 5}
b = {3, 4, 5, 6, 7, 8}

a &= b

print(a) # {3, 4, 5}
```

---

### Difference

If we have two sets - `a` and `b`, we can get the elements in `a` that are not in `b` using the `difference` method or `-` operator:

```py
a = {1, 2, 3, 4, 5}
b = {3, 4, 5, 6, 7, 8}

c = a.difference(b)
print(c) # {1, 2}

c = a - b
print(c) # {1, 2}
```

To update the original set, we can use the `difference_update` method or `-=` operator:

```py
a = {1, 2, 3, 4, 5}
b = {3, 4, 5, 6, 7, 8}

a.difference_update(b)

print(a) # {1, 2}
```

```py
a = {1, 2, 3, 4, 5}
b = {3, 4, 5, 6, 7, 8}

a -= b

print(a) # {1, 2}
```

---

### Symmetric difference

To get all of the elements in the set `a` or `b`, but not in both, we can use the `symmetric_difference` method or `^` operator:

```py
a = {1, 2, 3, 4, 5}
b = {3, 4, 5, 6, 7, 8}

c = a.symmetric_difference(b)
print(c) # {1, 2, 6, 7, 8}

c = a ^ b
print(c) # {1, 2, 6, 7, 8}
```

To update the original set, we can use the `symmetric_difference_update` method or `^=` operator:

```py
a = {1, 2, 3, 4, 5}
b = {3, 4, 5, 6, 7, 8}

a.symmetric_difference_update(b)

print(a) # {1, 2, 6, 7, 8}
```

```py
a = {1, 2, 3, 4, 5}
b = {3, 4, 5, 6, 7, 8}

a ^= b

print(a) # {1, 2, 6, 7, 8}
```

---

---

## `issubset`

We can check if the set `a` is the subset of set `b` (in other words, if all the elements of set `a` is contained within set `b`) using the `issubset` method or `<=` operator:

```py
a = {1, 2, 3, 4, 5}
b = {3, 4, 5, 6, 7, 8}
c = {1, 2, 3, 4, 5, 6, 7, 8, 9}

print(a.issubset(b)) # False
print(b.issubset(c)) # True

print(a <= b) # False
print(b <= c) # True
```

---

---

## `issuperset`

We can check if the set `a` is the superset of set `b` (in other words, if all the elements of `b` contained within set `a`) using the `issuperset` method or `>=` operator:

```py
a = {1, 2, 3, 4, 5}
b = {3, 4, 5, 6, 7, 8}
c = {1, 2, 3, 4, 5, 6, 7, 8, 9}

print(a.issuperset(b)) # False
print(c.issuperset(b)) # True

print(a >= b) # False
print(c >= b) # True
```

---

---

## `isdisjoint`

We can check if two sets have no common elements using the `isdisjoint` method:

```py
a = {1, 2, 3, 4, 5}
b = {6, 7, 8}

print(a.isdisjoint(b)) # True
```

---

---

## `add`

We can add an element to a set using the `add` method:

```py
a = {1, 2, 3, 4, 5}
a.add(6)

print(a) # {1, 2, 3, 4, 5, 6}
```

---

---

## `clear`

We can reset a set to an empty state, discarding all of its elements, by using the `clear` method:

```py
a = {1, 2, 3, 4, 5}
a.clear()

print(a) # set()
```

---

---

## Deleting set elements

We can remove an element from a set using the `remove` method:

```py
a = {1, 2, 3, 4, 5}
a.remove(3)

print(a) # {1, 2, 4, 5}
```

We can remove the first element from a set using the `pop` method. It will raise a `KeyError` if the set is empty:

```py
a = {1, 2, 3, 4, 5}
b = a.pop()

print(a) # {2, 3, 4, 5}
print(b) # 1
```

---

---

## Equality of sets

Sets are equal if and only if their contents are equal:

```py
print({1, 2, 3} == {3, 2, 1}) # True
```

---

---
