
# انواع متغیرها در پایتون

در پایتون، متغیرها برای ذخیره داده‌ها استفاده می‌شوند. پایتون یک زبان برنامه‌نویسی پویا است، به این معنی که نیازی به اعلان نوع متغیر نیست و نوع متغیر به صورت خودکار بر اساس مقدار اختصاص داده شده تعیین می‌شود. در اینجا به بررسی انواع مختلف متغیرها در پایتون می‌پردازیم:

## انواع متغیرها در پایتون

### 1. عددی (Numeric)
- **Integer (int)**: برای ذخیره اعداد صحیح.
  ```python
  age = 25
  ```
- **Floating Point (float)**: برای ذخیره اعداد اعشاری.
  ```python
  height = 5.9
  ```
- **Complex Number (complex)**: برای ذخیره اعداد مختلط.
  ```python
  complex_num = 2 + 3j
  ```

### 2. رشته‌ای (String)
- **String (str)**: برای ذخیره متن.
  ```python
  name = "Alice"
  ```

### 3. منطقی (Boolean)
- **Boolean (bool)**: برای ذخیره مقادیر منطقی درست (True) یا نادرست (False).
  ```python
  is_student = True
  ```

### 4. لیست (List)
- **List**: برای ذخیره مجموعه‌ای از مقادیر که قابل تغییر هستند.
  ```python
  fruits = ["apple", "banana", "cherry"]
  ```

### 5. تاپل (Tuple)
- **Tuple**: برای ذخیره مجموعه‌ای از مقادیر که قابل تغییر نیستند.
  ```python
  coordinates = (10.0, 20.0)
  ```

### 6. مجموعه (Set)
- **Set**: برای ذخیره مجموعه‌ای از مقادیر یکتا.
  ```python
  unique_numbers = {1, 2, 3, 4, 5}
  ```

### 7. دیکشنری (Dictionary)
- **Dictionary (dict)**: برای ذخیره جفت‌های کلید و مقدار.
  ```python
  student = {"name": "Alice", "age": 25, "is_student": True}
  ```

### 8. None
- **None**: برای نشان دادن عدم مقدار.
  ```python
  unknown = None
  ```

## نمونه کد

در زیر یک نمونه کد شامل انواع مختلف متغیرها در پایتون آورده شده است:

```python
# Integer
age = 25

# Float
height = 5.9

# Complex
complex_num = 2 + 3j

# String
name = "Alice"

# Boolean
is_student = True

# List
fruits = ["apple", "banana", "cherry"]

# Tuple
coordinates = (10.0, 20.0)

# Set
unique_numbers = {1, 2, 3, 4, 5}

# Dictionary
student = {"name": "Alice", "age": 25, "is_student": True}

# None
unknown = None

# Printing the variables
print("Age:", age)
print("Height:", height)
print("Complex Number:", complex_num)
print("Name:", name)
print("Is Student:", is_student)
print("Fruits:", fruits)
print("Coordinates:", coordinates)
print("Unique Numbers:", unique_numbers)
print("Student:", student)
print("Unknown:", unknown)
```

## توضیحات اضافی
- **نوع متغیرها را می‌توانید با استفاده از تابع `type()` بررسی کنید**:
  ```python
  print(type(age))  # <class 'int'>
  print(type(height))  # <class 'float'>
  print(type(complex_num))  # <class 'complex'>
  print(type(name))  # <class 'str'>
  print(type(is_student))  # <class 'bool'>
  print(type(fruits))  # <class 'list'>
  print(type(coordinates))  # <class 'tuple'>
  print(type(unique_numbers))  # <class 'set'>
  print(type(student))  # <class 'dict'>
  print(type(unknown))  # <class 'NoneType'>
  ```

این راهنما شامل انواع مختلف متغیرها در پایتون و نمونه‌هایی از هر کدام است که به شما کمک می‌کند تا با استفاده از این متغیرها برنامه‌های خود را به طور مؤثرتری بنویسید.
