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


