# Python Variables and Data Types

In Python, variables are used to store data that can be used later in the program. Python supports several data types, each serving different purposes. This document covers the basics of variables and data types in Python.

## 1. Variables

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

## 2. Data Types

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

## Conclusion

Understanding variables and data types is fundamental in Python programming. They allow you to store and manipulate data effectively. By mastering these basics, you'll be well-prepared to tackle more complex programming challenges.
