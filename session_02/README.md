# Python Fundamentals for Data Science & Machine Learning (Part 02)

This repository contains a comprehensive guide to **Python Fundamentals**, specifically tailored for Data Science and Machine Learning. It covers essential concepts from basic variable tracking to advanced string manipulation and conditional logic.

## 📋 Table of Contents
- [1. Tracking Variables](#1-tracking-variables)
- [2. Conditional Statements](#2-conditional-statements)
- [3. Type Conversion](#3-type-conversion)
- [4. Operators](#4-operators)
- [5. Numeric & String Functions](#5-numeric--string-functions)
- [6. String Indexing & Slicing](#6-string-indexing--slicing)
- [7. String Methods](#7-string-methods)
- [8. F-Strings & Docstrings](#8-f-strings--docstrings)

---

## 1. Tracking Variables
In interactive environments like Jupyter or Google Colab, you can use **Magic Commands** to keep track of your variables.

| Command | Description |
| :--- | :--- |
| `%who` | Lists all variable names currently in the namespace. |
| `%whos` | Provides a detailed table including variable names, types, and data info. |

**Example:**
```python
price = 10
product = 'Super Snowboard'
Date = '10-Jan-2021'
dimensions = [160, 25, 2]

# %who returns variable names
%who
# Output: Date dimensions price product

# %whos returns variable names, types, and detailed information
%whos
```

---

## 2. Conditional Statements
Conditional statements allow your code to make decisions based on specific criteria.

**Syntax:**
```python
if condition1:
    # Code to execute if condition1 is True
elif condition2:
    # Code to execute if condition2 is True
else:
    # Code to execute if all conditions are False
```

**Example: Conditional Statements**
```python
age = 18
if age < 13:
    print("You are a child.")
elif age < 20:
    print("You are a teenager.")
else:
    print("You are an adult.")
# Output: You are a teenager.
```

---

## 3. Type Conversion
Converting data from one type to another is crucial for data processing.

- `int()`, `float()`, `str()`, `list()`, `set()`

**Example: Type Conversion**
```python
# Convert a string to an integer
salary_str = "10000"
salary_int = int(salary_str)
print(f"Type after conversion: {type(salary_int)}") # Output: <class 'int'>

# Convert a list to a set to remove duplicates
duplicate_list = [1, 2, 4, 3, 3]
unique_set = set(duplicate_list)
print(unique_set) # Output: {1, 2, 3, 4}

# Check length of set vs list
print(len(duplicate_list)) # Output: 5
print(len(unique_set))     # Output: 4
```

---

## 4. Operators
### Arithmetic Operators
Used for mathematical calculations.

| Operator | Name | Example | Result |
| :--- | :--- | :--- | :--- |
| `+` | Addition | `10 + 3` | `13` |
| `-` | Subtraction | `10 - 3` | `7` |
| `*` | Multiplication | `10 * 3` | `30` |
| `/` | Division | `10 / 3` | `3.33...` |
| `//` | Floor Division | `10 // 3` | `3` |
| `%` | Modulus | `10 % 3` | `1` |
| `**` | Exponentiation | `10 ** 3` | `1000` |

### Comparison & Logical Operators
Used for evaluation and combining conditions.
- **Comparison:** `==`, `!=`, `>`, `<`, `>=`, `<=`
- **Logical:** `and`, `or`, `not`

**Example: Comparison & Logical Operators**
```python
x = 10
y = 20
print(f"Is x equal to y? {x == y}") # Output: False
print(f"Is x less than or equal to y? {x <= y}") # Output: True

is_student = True
is_working = False
print(f"Is student and working? {is_student and is_working}") # Output: False
print(f"Is student or working? {is_student or is_working}")   # Output: True
```

---

## 5. Numeric & String Functions
Built-in functions to perform quick operations on data.

**Example: Numeric Functions**
```python
print(f"Absolute value of -10: {abs(-10)}") # Output: 10
print(f"Rounded value of 3.14159: {round(3.14159, 2)}") # Output: 3.14
print(f"Minimum of [5, 2, 8]: {min([5, 2, 8])}") # Output: 2
```

**Example: String Functions**
```python
text = "Hello, World!"
print(f"Length of text: {len(text)}") # Output: 13
print(f"Number as string: {str(100)}") # Output: '100'
```

---

## 6. String Indexing & Slicing
Access specific parts of a string using indices.

- **Indexing:** `text[0]` (First character)
- **Slicing:** `text[start:end:step]`
- **Reverse:** `text[::-1]`

**Example: String Indexing & Slicing**
```python
text = "Python Programming"
print(f"First character: {text[0]}")        # Output: P
print(f"Substring (7 to 11): {text[7:12]}") # Output: Progr
print(f"Every second character: {text[::2]}") # Output: Pto rgamn
print(f"Reverse string: {text[::-1]}")      # Output: gnimmargorP nohtyP
```

---

## 7. String Methods
Methods are functions that belong to the string class and help in text cleaning.

| Method | Description |
| :--- | :--- |
| `.lower()` / `.upper()` | Change case. |
| `.strip()` | Remove leading/trailing whitespace or characters. |
| `.replace(old, new)` | Swap substrings. |
| `.split(separator)` | Break string into a list. |
| `"".join(list)` | Combine list into a string. |

**Example: String Methods**
```python
text = "  Hello, World!  "
print(f"Lowercase: {text.lower()}")
print(f"Stripped: '{text.strip()}'") # Output: 'Hello, World!'
print(f"Replaced: {text.replace('World', 'Python')}") # Output:   Hello, Python!  

# Data Cleaning Example
salary = '$10000'
clean_salary = int(salary.strip('$'))
print(f"Cleaned Salary (int): {clean_salary}") # Output: 10000
```

---

## 8. F-Strings & Docstrings
### F-Strings
A modern way to format strings by embedding expressions inside `{}`.

**Example: F-Strings**
```python
name = "Rossi"
age = 34
print(f"My name is {name} and I am {age} years old.")
print(f"Next year, I will be {age + 1} years old.")
```

### Docstrings
Used for documenting functions, classes, and modules.

**Example: Docstring**
```python
def calculate_area(length, width):
    """
    Calculates the area of a rectangle.

    Args:
        length (float): The length of the rectangle.
        width (float): The width of the rectangle.

    Returns:
        float: The calculated area of the rectangle.
    """
    return length * width
```

---

---
*This documentation was generated to provide a clear overview of Python fundamentals for data science applications.*
