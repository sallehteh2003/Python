# Object-Oriented Programming in Python

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


