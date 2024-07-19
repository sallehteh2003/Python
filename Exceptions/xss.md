# Error Handling in Python

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
