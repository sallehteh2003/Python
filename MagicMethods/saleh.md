# Magic Methods and Operator Overloading in Python

## Introduction

Magic methods in Python are special methods that you can define to add "magic" to your classes. They are always surrounded by double underscores (e.g., `__init__`, `__str__`, `__add__`). Magic methods allow you to define the behavior of your objects for built-in operations and functions. One of the key uses of magic methods is operator overloading, where you can define custom behavior for operators like `+`, `-`, `*`, etc.

## Common Magic Methods

### `__init__(self, ...)`
The initializer method, called when a new instance of the class is created.

```python
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

p = Person("Alice", 30)
```

### `__str__(self)`
Returns a string representation of the object, used by `print()` and `str()`.

```python
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def __str__(self):
        return f"{self.name}, {self.age} years old"

p = Person("Alice", 30)
print(p)  # Output: Alice, 30 years old
```

### `__repr__(self)`
Returns an official string representation of the object, used by `repr()` and often by the interactive interpreter.

```python
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def __repr__(self):
        return f"Person(name={self.name}, age={self.age})"

p = Person("Alice", 30)
print(repr(p))  # Output: Person(name=Alice, age=30)
```

## Operator Overloading

### `__add__(self, other)`
Defines the behavior of the `+` operator.

```python
class Vector:
    def __init__(self, x, y):
        self.x = x
        self.y = y

    def __add__(self, other):
        return Vector(self.x + other.x, self.y + other.y)

    def __str__(self):
        return f"Vector({self.x}, {self.y})"

v1 = Vector(2, 3)
v2 = Vector(5, 7)
print(v1 + v2)  # Output: Vector(7, 10)
```

### `__sub__(self, other)`
Defines the behavior of the `-` operator.

```python
class Vector:
    def __init__(self, x, y):
        self.x = x
        self.y = y

    def __sub__(self, other):
        return Vector(self.x - other.x, self.y - other.y)

    def __str__(self):
        return f"Vector({self.x}, {self.y})"

v1 = Vector(5, 7)
v2 = Vector(2, 3)
print(v1 - v2)  # Output: Vector(3, 4)
```

### `__mul__(self, other)`
Defines the behavior of the `*` operator.

```python
class Vector:
    def __init__(self, x, y):
        self.x = x
        self.y = y

    def __mul__(self, scalar):
        return Vector(self.x * scalar, self.y * scalar)

    def __str__(self):
        return f"Vector({self.x}, {self.y})"

v = Vector(2, 3)
print(v * 3)  # Output: Vector(6, 9)
```

### `__truediv__(self, other)`
Defines the behavior of the `/` operator.

```python
class Vector:
    def __init__(self, x, y):
        self.x = x
        self.y = y

    def __truediv__(self, scalar):
        return Vector(self.x / scalar, self.y / scalar)

    def __str__(self):
        return f"Vector({self.x}, {self.y})"

v = Vector(6, 9)
print(v / 3)  # Output: Vector(2.0, 3.0)
```

### `__eq__(self, other)`
Defines the behavior of the `==` operator.

```python
class Vector:
    def __init__(self, x, y):
        self.x = x
        self.y = y

    def __eq__(self, other):
        return self.x == other.x and self.y == other.y

v1 = Vector(2, 3)
v2 = Vector(2, 3)
v3 = Vector(3, 4)
print(v1 == v2)  # Output: True
print(v1 == v3)  # Output: False
```

### `__lt__(self, other)`
Defines the behavior of the `<` operator.

```python
class Vector:
    def __init__(self, x, y):
        self.x = x
        self.y = y

    def __lt__(self, other):
        return (self.x**2 + self.y**2) < (other.x**2 + other.y**2)

v1 = Vector(2, 3)
v2 = Vector(3, 4)
print(v1 < v2)  # Output: True
```

## Conclusion

Magic methods and operator overloading in Python allow you to define custom behavior for your classes in a natural and intuitive way. By understanding and using these methods, you can create more powerful and flexible objects.

