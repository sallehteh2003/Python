# Python

How Learn Python Without Course And Teacher 

## Python Introduction
Python is a popular programming language. It was created by Guido van Rossum, and released in 1991.

#### Python used for :
- **web development (server-side)**
- **software development**
- **mathematics**
- **system scripting**

### Python Main Concepts

- **Variable AND Data Types**
- **Control Flow**
- **Class AND Object-Oriented-Programming (OOP)**
- **Error Handling AND Exceptions**
- **Magic Methods and Operator Overloading**
- **Modules and Packages**

# 1. Python Variables and Data Types

In Python, variables are used to store data that can be used later in the program. Python supports several data types, each serving different purposes. This document covers the basics of variables and data types in Python.

## 1.1 Variables

Variables in Python are created by assigning a value to a variable name using the equals sign (`=`).

```python
x = 5
name = "Alice"
is_valid = True
```

### Variable Naming Rules

1. Variable names must start with a letter or an underscore.
2. The rest of the name can contain letters, numbers, and underscores.
3. Variable names are case-sensitive (e.g., `myVar` and `myvar` are different variables).

## 1.2 Data Types

Python supports several data types. The most commonly used ones include:

### Integer

Integers are whole numbers, positive or negative, without decimals.

```python
age = 25
year = 2021
```

### Float

Floats are numbers that contain a decimal point.

```python
price = 19.99
pi = 3.14159
```

### String

Strings are sequences of characters, enclosed in single or double quotes.

```python
greeting = "Hello, World!"
name = 'Alice'
```

### Boolean

Booleans represent one of two values: `True` or `False`.

```python
is_valid = True
has_error = False
```

### List

 Lists are ordered collections of items, which can be of different types. Lists are mutable, meaning their contents can be changed.

 ```python
 fruits = ["apple", "banana", "cherry"]
 numbers = [1, 2, 3, 4, 5]
 mixed = [1, "hello", 3.14, True]
 ```

 #### How Make List :


 ```python
 numbers = list(range(0,5))
 # use func list [ 0,1,2,3,4 ]
 emptyList = [] * 10
 # []
 myList = [ value for value in range(0,10) ] 
 # [ 0,1,2,3,4,5,6,7,8,9 ]
 MYList = [0] * 10
 # [ 0,0,0,0,0,0,0,0,0,0 ]
 ```
### Python List Methods

Python lists are one of the most versatile and commonly used data structures. Lists are ordered collections of items, which can be of any type. Python provides a variety of methods to work with lists effectively.

<details>
  <summary>Append</summary>
  
  ### `append()`
  
  Adds an item to the end of the list.
  
  ```python
  fruits = ['apple', 'banana', 'cherry']
  fruits.append('orange')
  print(fruits)  # Output: ['apple', 'banana', 'cherry', 'orange']
  ```
  
</details>

<details>
  <summary>Extend</summary>
  
  ### `extend()`
  
  Extends the list by appending all the items from the iterable.
  
  ```python
  fruits = ['apple', 'banana', 'cherry']
  fruits.extend(['mango', 'pineapple'])
  print(fruits)  # Output: ['apple', 'banana', 'cherry', 'mango', 'pineapple']
  ```
  
</details>

<details>
  <summary>Insert</summary>
  
  ### `insert()`
  
  Inserts an item at a given position.
  
  ```python
  fruits = ['apple', 'banana', 'cherry']
  fruits.insert(1, 'orange')
  print(fruits)  # Output: ['apple', 'orange', 'banana', 'cherry']
  ```
  
</details>

<details>
  <summary>Remove</summary>
  
  ### `remove()`
  
  Removes the first item from the list whose value is equal to the specified value.
  
  ```python
  fruits = ['apple', 'banana', 'cherry', 'banana']
  fruits.remove('banana')
  print(fruits)  # Output: ['apple', 'cherry', 'banana']
  ```
  
</details>

<details>
  <summary>POP</summary>
  
  ### `pop()`
  
  Removes and returns the item at the given position. If no index is specified, it removes and returns the last item.
  
  ```python
  fruits = ['apple', 'banana', 'cherry']
  fruit = fruits.pop(1)
  print(fruit)   # Output: banana
  print(fruits)  # Output: ['apple', 'cherry']
  ```
  
</details>

<details>
  <summary>Clear</summary>
  
  ### `clear()`
  
  Removes all items from the list.
  
  ```python
  fruits = ['apple', 'banana', 'cherry']
  fruits.clear()
  print(fruits)  # Output: []
  ```
  
</details>

<details>
  <summary>Index</summary>
  
  ### `index()`
  
  Returns the index of the first item whose value is equal to the specified value.
  
  ```python
  fruits = ['apple', 'banana', 'cherry']
  index = fruits.index('cherry')
  print(index)  # Output: 2
  ```
  
</details>

<details>
  <summary>Count</summary>
  
  ### `count()`
  
  Returns the number of times the specified item appears in the list.
  
  ```python
  fruits = ['apple', 'banana', 'cherry', 'banana']
  count = fruits.count('banana')
  print(count)  # Output: 2
  ```
  
</details>

<details>
  <summary>Sort</summary>
  
  ### `sort()`
  
  Sorts the items of the list in ascending order by default.
  
  ```python
  numbers = [3, 1, 4, 1, 5, 9, 2, 6, 5]
  numbers.sort()
  print(numbers)  # Output: [1, 1, 2, 3, 4, 5, 5, 6, 9]
  ```
  
  To sort in descending order:
  
  ```python
  numbers.sort(reverse=True)
  print(numbers)  # Output: [9, 6, 5, 5, 4, 3, 2, 1, 1]
  ```
  
</details>

<details>
  <summary>Reverse</summary>
  
  ### `reverse()`
  
  Reverses the items of the list in place.
  
  ```python
  fruits = ['apple', 'banana', 'cherry']
  fruits.reverse()
  print(fruits)  # Output: ['cherry', 'banana', 'apple']
  ```
  
</details>

<details>
  <summary>Copy</summary>
  
  ### `copy()`
  
  Returns a shallow copy of the list.
  
  ```python
  fruits = ['apple', 'banana', 'cherry']
  fruits_copy = fruits.copy()
  print(fruits_copy)  # Output: ['apple', 'banana', 'cherry']
  ```
  
</details>



### Tuple

Tuples are similar to lists, but they are immutable, meaning their contents cannot be changed after creation.

```python
coordinates = (10, 20)
colors = ("red", "green", "blue")
```

### Dictionary

Dictionaries are collections of key-value pairs, where each key is unique. They are unordered and mutable.

```python
person = {
    "name": "Alice",
    "age": 25,
    "city": "New York"
}
```

### Set

Sets are unordered collections of unique items.

```python
unique_numbers = {1, 2, 3, 4, 5}
unique_fruits = {"apple", "banana", "cherry"}
```

## 3. Type Conversion

You can convert between data types using built-in functions.

```python
# Convert integer to float
x = 10
y = float(x)  # y is 10.0

# Convert float to integer
pi = 3.14
radius = int(pi)  # radius is 3

# Convert integer to string
age = 25
age_str = str(age)  # age_str is "25"

# Convert string to integer
num_str = "100"
num = int(num_str)  # num is 100
```
## 4. Constructor functions of ( List , Tuple , Dictionary , Set )

```python
# Using the list() constructor to make a List:
thislist = list(("apple", "banana", "cherry")) # note the double round-brackets

# It is also possible to use the tuple() constructor to make a tuple.
thistuple = tuple(("apple", "banana", "cherry")) # note the double round-brackets

# It is also possible to use the set() constructor to make a set.
thisset = set(("apple", "banana", "cherry")) # note the double round-brackets

# It is also possible to use the dict() constructor to make a dictionary.
thisdict = dict(name = "John", age = 36, country = "Norway")
```

## Conclusion

Understanding variables and data types is fundamental in Python programming. They allow you to store and manipulate data effectively. By mastering these basics, you'll be well-prepared to tackle more complex programming challenges.

# 2. Python Control Flow

Control flow in Python refers to the order in which the instructions in a program are executed. Python provides several control flow tools to help you write code that can make decisions, repeat actions, and more. In this document, we will cover `if`, `elif`, `else`, `for`, and `while`.

## 1. if Statement

The `if` statement is used to test a condition. If the condition is true, the code block under the `if` statement is executed.

```python
x = 10

if x > 5:
    print("x is greater than 5")
```

## 2. elif Statement

The `elif` statement is short for "else if" and allows you to check multiple expressions for `True` and execute a block of code as soon as one of the conditions is true.

```python
x = 10

if x > 10:
    print("x is greater than 10")
elif x == 10:
    print("x is equal to 10")
else:
    print("x is less than 10")
```

## 3. else Statement

The `else` statement catches anything which isn't caught by the preceding conditions.

```python
x = 5

if x > 10:
    print("x is greater than 10")
elif x == 10:
    print("x is equal to 10")
else:
    print("x is less than 10")
```

## 4. for Loop

The `for` loop in Python is used to iterate over a sequence (such as a list, tuple, string, or range).

```python
# Example with a list
numbers = [1, 2, 3, 4, 5]

for number in numbers:
    print(number)

# Example with a range
for i in range(5):
    print(i)
```

## 5. while Loop

The `while` loop in Python is used to execute a block of code as long as the condition is true.

```python
count = 0

while count < 5:
    print(count)
    count += 1
```

## 6. Break and Continue

### break Statement

The `break` statement is used to exit a loop prematurely.

```python
for i in range(10):
    if i == 5:
        break
    print(i)
```

### continue Statement

The `continue` statement is used to skip the current iteration of a loop and proceed to the next iteration.

```python
for i in range(10):
    if i % 2 == 0:
        continue
    print(i)
```

## 7. Nested Loops

Loops can be nested within each other to create more complex control flows.

```python
for i in range(3):
    for j in range(3):
        print(f"i: {i}, j: {j}")
```

## Conclusion

Control flow statements are fundamental to programming in Python. They allow you to direct the execution of your code based on conditions and repeat actions efficiently. By mastering `if`, `elif`, `else`, `for`, `while`, `break`, and `continue`, you'll be well-equipped to handle a wide variety of programming tasks.

# 3. Error Handling in Python

Error handling is a crucial aspect of programming that allows you to manage and respond to runtime errors in a controlled way. Python provides several constructs for handling errors and exceptions.

## 1. `try` and `except`

The `try` block lets you test a block of code for errors. The `except` block lets you handle the error.

### Basic Syntax

```python
try:
    # Code that might raise an exception
    risky_code()
except SomeException as e:
    # Code that runs if an exception occurs
    handle_exception(e)
```

### Example

```python
try:
    x = 1 / 0
except ZeroDivisionError as e:
    print(f"Error occurred: {e}")
```

### Multiple Exceptions

You can handle multiple exceptions by specifying multiple `except` blocks.

```python
try:
    x = int("hello")
except ValueError as ve:
    print(f"Value error: {ve}")
except TypeError as te:
    print(f"Type error: {te}")
```

## 2. `else` and `finally`

The `else` block lets you run code if no exceptions were raised. The `finally` block lets you execute code regardless of whether an exception was raised or not.

### Example

```python
try:
    result = 10 / 2
except ZeroDivisionError as e:
    print(f"Error: {e}")
else:
    print("No errors occurred.")
finally:
    print("This code runs no matter what.")
```

## 3. Raising Exceptions

You can raise exceptions in your code using the `raise` statement.

### Syntax

```python
raise SomeException("Error message")
```

### Example

```python
def divide(a, b):
    if b == 0:
        raise ValueError("Cannot divide by zero")
    return a / b

try:
    result = divide(10, 0)
except ValueError as e:
    print(f"Error: {e}")
```

## 4. Custom Exceptions

You can define custom exceptions by creating a new class that inherits from the `Exception` class.

### Example

```python
class CustomError(Exception):
    pass

def risky_function():
    raise CustomError("This is a custom error")

try:
    risky_function()
except CustomError as e:
    print(f"Caught custom exception: {e}")
```

## Conclusion

Proper error handling ensures your programs can gracefully handle unexpected situations. By using `try`, `except`, `else`, `finally`, and custom exceptions, you can create robust and resilient Python applications.

# 4. Object-Oriented Programming in Python

Object-Oriented Programming (OOP) is a programming paradigm based on the concept of "objects" which can contain data and methods. Python is an object-oriented programming language that allows you to define and use classes and objects.

## 1. Classes and Objects

A class is a blueprint for creating objects. Objects are instances of classes.

### Basic Syntax

```python
class MyClass:
    def __init__(self, name):
        self.name = name

    def greet(self):
        print(f"Hello, {self.name}!")

# Creating an object
obj = MyClass("Alice")
obj.greet()
```

## 2. Inheritance

Inheritance allows a class to inherit attributes and methods from another class. The class being inherited from is called the base class or parent class, and the class that inherits is called the derived class or child class.

### Example

```python
class Animal:
    def __init__(self, name):
        self.name = name

    def speak(self):
        pass

class Dog(Animal):
    def speak(self):
        return f"{self.name} says Woof!"

class Cat(Animal):
    def speak(self):
        return f"{self.name} says Meow!"

dog = Dog("Buddy")
cat = Cat("Whiskers")

print(dog.speak())
print(cat.speak())
```
### Super Function :
The super() function returns an object that represents the parent class 
```python
class Animal:
    def __init__(self, name):
        self.name = name

    def speak(self):
        pass

class Dog(Animal):
    def __init__(self, name, age):
        self.age = age
        super().__init__(name)

    def speak(self):
        return f"{self.name} says Woof!"

class Cat(Animal):
    def __init__(self, name, age):
        super().__init__(name)
        self.age = age
    def speak(self):
        return f"{self.name} says Meow!"

dog = Dog("Buddy",10)
cat = Cat("Whiskers",5)

print(dog.speak())
print(cat.speak())
```

## 3. Polymorphism

Polymorphism allows methods to do different things based on the object it is acting upon. It is commonly used in methods that can work with objects of different classes.

### Example

```python
class Bird:
    def fly(self):
        return "Bird is flying"

class Airplane:
    def fly(self):
        return "Airplane is flying"

def let_fly(flying_object):
    print(flying_object.fly())

bird = Bird()
airplane = Airplane()

let_fly(bird)
let_fly(airplane)
```

## 4. Abstract Classes

Abstract classes are classes that contain one or more abstract methods. An abstract method is a method that is declared, but contains no implementation. Abstract classes cannot be instantiated directly.

### Example

```python
from abc import ABC, abstractmethod

class Shape(ABC):
    @abstractmethod
    def area(self):
        pass

class Circle(Shape):
    def __init__(self, radius):
        self.radius = radius

    def area(self):
        return 3.14 * self.radius * self.radius

circle = Circle(5)
print(circle.area())
```

## 5. Constructors

A constructor is a special method called when an object is instantiated. In Python, the `__init__` method is used as the constructor.

### Example

```python
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def display(self):
        print(f"Name: {self.name}, Age: {self.age}")

person = Person("Alice", 30)
person.display()
```

## 6. Getters and Setters

Getters and setters are methods that allow you to access and modify the attributes of an object. In Python, you can use the `property` decorator to create getters and setters.

### Example

```python
class Employee:
    def __init__(self, name, salary):
        self._name = name
        self._salary = salary

    @property
    def name(self):
        return self._name

    @name.setter
    def name(self, value):
        self._name = value

    @property
    def salary(self):
        return self._salary

    @salary.setter
    def salary(self, value):
        if value < 0:
            raise ValueError("Salary cannot be negative")
        self._salary = value

employee = Employee("Bob", 50000)
print(employee.name)
employee.salary = 55000
print(employee.salary)
```

## Conclusion

Object-oriented programming in Python is a powerful way to structure your code. By using classes, inheritance, polymorphism, abstract classes, constructors, getters, and setters, you can write clean and maintainable code that models real-world objects and relationships.

# 5. Magic Methods and Operator Overloading in Python

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

# 6. Modules and Packages in Python

## Introduction

In Python, modules and packages are used to organize and reuse code. This document explains the concepts of modules and packages, how to import them, and how to create your own packages.

## Modules

A module is a single file containing Python definitions and statements. Modules can define functions, classes, and variables, and can also include runnable code.

### Creating a Module

To create a module, simply save the code you want in a file with a `.py` extension. For example, create a file named `mymodule.py` with the following content:

```python
# mymodule.py

def greet(name):
    return f"Hello, {name}!"

PI = 3.14159
```

### Importing a Module

You can import a module using the `import` statement. Once imported, you can use the module's functions, classes, and variables.

```python
import mymodule
# also we can use this code
from mymodule import *

print(mymodule.greet("Alice"))  # Output: Hello, Alice!
print(mymodule.PI)  # Output: 3.14159
```

### Importing Specific Elements

You can also import specific elements from a module using the `from ... import ...` syntax:

```python
from mymodule import greet, PI

print(greet("Bob"))  # Output: Hello, Bob!
print(PI)  # Output: 3.14159
```

### Using Aliases

You can use aliases to rename modules or elements when importing:

```python
import mymodule as mm

print(mm.greet("Charlie"))  # Output: Hello, Charlie!

from mymodule import greet as hello

print(hello("Dave"))  # Output: Hello, Dave!
```

## Packages

A package is a way of organizing multiple modules. A package is a directory that contains a special `__init__.py` file and can contain sub-packages and modules.

### Creating a Package

To create a package, follow these steps:

1. Create a directory for the package.
2. Create an `__init__.py` file inside the directory.
3. Add modules to the package directory.

Example directory structure:

```
mypackage/
    __init__.py
    module1.py
    module2.py
```

### Importing from a Package

You can import modules from a package using the `import` statement:

```python
import mypackage.module1
import mypackage.module2

print(mypackage.module1.some_function())
print(mypackage.module2.some_variable)
```

### Using `__init__.py`

The `__init__.py` file can be used to initialize a package and define what is exported when the package is imported.

```python
# mypackage/__init__.py

from .module1 import some_function
from .module2 import some_variable

__all__ = ["some_function", "some_variable"]
```

Now you can import directly from the package:

```python
from mypackage import some_function, some_variable

print(some_function())
print(some_variable)
```

## Creating and Installing Packages

To distribute and install packages, you can use tools like `setuptools`. Here’s a simple example of how to create a distributable package:

1. Create a `setup.py` file in the root directory of your package:

```python
# setup.py

from setuptools import setup, find_packages

setup(
    name="mypackage",
    version="0.1",
    packages=find_packages(),
)
```

2. Build and install the package:

```sh
python setup.py sdist
pip install .
```

## Conclusion

Modules and packages are powerful tools in Python for organizing and reusing code. By understanding how to create and import them, you can structure your projects more effectively and make your code more modular and maintainable.


