# Python Control Flow

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


