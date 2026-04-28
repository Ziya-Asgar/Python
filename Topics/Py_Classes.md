# Classes

- [Classes](#classes)
  - [Creating a class and an object instance](#creating-a-class-and-an-object-instance)
  - [Accessing class members with `getattr`](#accessing-class-members-with-getattr)
  - [Name mangling and naming convention for private class members](#name-mangling-and-naming-convention-for-private-class-members)
  - [Class attributes vs instance attributes](#class-attributes-vs-instance-attributes)
  - [`__dict__` attribute](#__dict__-attribute)

---

---

In Python, **attributes** are variables defined inside a class. **Methods** are functions that you define within a class. Attributes and methods are collectively referred to as **members** of a class or object.

---

---

## Creating a class and an object instance

- To define a class, you need to use the `class` keyword followed by the class name and a colon.
- The `.__init__()` method, inside classes, is known as the object initializer because it defines and sets the initial values for your attributes.
- The first argument of the most methods is `self`. This argument holds a reference to the current object so that you can use it inside a class.

Here is an example of creating a class:

```py
class ClassName:
  def __init__(self, someVariable):
    self.someVariable = someVariable
    self.anotherVariable = 'some data'

  def printData(self):
    print(self.someVariable)
```

Here is how we create an object instance from a class constructor:

```py
newObj = ClassName("something")
newObj.printData() # something
print(newObj.anotherVariable) # some data

newObj2 = ClassName("another thing")
newObj2.printData() # another thing
print(newObj2.anotherVariable) # some data
```

---

---

## Accessing class members with `getattr`

Attributes and methods can also be accessed by name via the `getattr` function:

```py
class ClassName:
  def __init__(self, someVariable):
    self.someVariable = someVariable
    self.anotherVariable = 'some data'

  def printData(self):
    print(self.someVariable)

  var = "variable"


print(getattr(ClassName, "printData")) # <function ClassName.printData at 0x00000287F35993A0>
print(getattr(ClassName, "var")) # variable
```

---

---

## Name mangling and naming convention for private class members

In Python, all attributes are accessible in one way or another. However, Python has a well-established naming convention that you should use to communicate that an attribute or method isn’t intended for use from outside its containing class or object. The naming convention consists of adding a leading underscore to the member’s name. A variable named `_variable` in a class is a non-public variable.

Another naming convention that you need to take into account in Python classes is adding two leading underscores to attribute and method names. This naming convention triggers what’s known as **name mangling**. Name mangling is an automatic name transformation that prepends the class’s name to the member’s name. For example, `__attribute` becomes `_ClassName__attribute` or `__method` becomes `_ClassName__method`. It’s a way to avoid naming conflicts between classes or subclasses.

```py
class ClassName:
  def __init__(self, someVariable):
    self.someVariable = someVariable

  def __some_method(self):
    return print(self.someVariable)

newObj = ClassName("Hello")
newObj._ClassName__some_method() # Hello
newObj.__some_method() # AttributeError: 'ClassName' object has no attribute '__some_method'
```

---

---

## Class attributes vs instance attributes

In Python, there are instance and class attributes.

**Instance attributes** are shared between different instances of a class and they are accessed using `self` inside the class. The `self` argument holds a reference to the current instance, which is where the attributes belong and live.

In the below example, the `Car` class have several instance attributes that will be available in all the instances of the `Car` class. Note how the values of the associated attributes are different and specific to the concrete instance:

```py
class Car:
  def __init__(self, brand, year):
    # instance attributes
    self.brand = brand
    self.year = year
    self.max_speed = 200

newCar = Car("Togg", 2024)
print(newCar.brand, newCar.year, newCar.max_speed)
# Togg 2024 200

newCar2 = Car("Togg", 2020)
print(newCar2.brand, newCar2.year, newCar2.max_speed)
# Togg 2020 200
```

**Class attributes** are variables that you define directly in the class body but outside of any method. These attributes are tied to the class itself rather than to particular instances of that class. If you change a class attribute, that change affects all the derived objects.

```py
class ObjectCounter:
  # class attributes
  num_instances = 0

  def __init__(self):
    ObjectCounter.num_instances += 1

ObjectCounter()
ObjectCounter()
counter = ObjectCounter()
counter2 = ObjectCounter()

print(ObjectCounter.num_instances) # 4
print(counter.num_instances) # 4
print(counter2.num_instances) # 4
```

It’s important to note that you can access class attributes using either the class or one of its instances. That’s why you can use the `counter` object to retrieve the value of `.num_instances`. However, if you need to modify a class attribute, then you must use the class itself rather than one of its instances.

```py
class ObjectCounter:
  num_instances = 0

  def __init__(self):
    ObjectCounter.num_instances += 1

ObjectCounter()
counter = ObjectCounter()

print(ObjectCounter.num_instances) # 2
print(counter.num_instances) # 2

ObjectCounter.num_instances = 10
print(ObjectCounter.num_instances) # 10
print(counter.num_instances) # 10

counter.num_instances = 100
print(ObjectCounter.num_instances) # 10
print(counter.num_instances) # 100
```

In general, you should use class attributes for sharing data between instances of a class. Any changes on a class attribute will be visible to all the instances of that class.

---

---

## `__dict__` attribute

In Python, both classes and instances have a special attribute called `__dict__`. This attribute holds a dictionary containing the writable members of the underlying class or instance. Remember that:

- `__dict__` used on a class shows all the class attributes and methods.
- `__dict__` used on an instance shows only the instance attributes and methods.

```py
class SampleClass:
  class_attr = 100

  def __init__(self, instance_attr):
    self.instance_attr = instance_attr

  def method(self):
    print(f"Class attribute: {self.class_attr}")
    print(f"Instance attribute: {self.instance_attr}")

print(SampleClass.__dict__)
print(SampleClass.__dict__['class_attr']) # 100
print(SampleClass.__dict__['method']) # <function SampleClass.method at 0x00000197A48493A0>

sample = SampleClass("instance")
print(sample.__dict__) # {'instance_attr': 'instance'}
```

---

---
