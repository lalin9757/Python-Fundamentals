# Python Fundamentals for Data Science & Machine Learning

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
- [🚀 Practice Exercises](#-practice-exercises)

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
%who
# Output: price product
```

---

## 2. Conditional Statements
Conditional statements allow your code to make decisions based on specific criteria.

**Syntax:**
```python
if condition1:
    # Code for condition1
elif condition2:
    # Code for condition2
else:
    # Default code
```

**Real-life Use Case:** Age-based categorization or validating user input.

---

## 3. Type Conversion
Converting data from one type to another is crucial for data processing (e.g., converting a string price like `"$100"` to an integer `100`).

- `int()`: Convert to Integer
- `float()`: Convert to Float
- `str()`: Convert to String
- `list()`: Convert to List
- `set()`: Convert to Set (removes duplicates)

**Example:**
```python
unique_numbers = set([1, 2, 2, 3, 4, 4])
# Result: {1, 2, 3, 4}
```

---

## 4. Operators
### Arithmetic Operators
Used for mathematical calculations.
- `+`, `-`, `*`, `/` : Basic Math
- `//` : Floor Division (rounds down)
- `%` : Modulus (remainder)
- `**` : Exponentiation (power)

### Comparison & Logical Operators
Used for evaluation and combining conditions.
- **Comparison:** `==`, `!=`, `>`, `<`, `>=`, `<=`
- **Logical:** `and`, `or`, `not`

---

## 5. Numeric & String Functions
Built-in functions to perform quick operations on data.

| Function | Type | Description |
| :--- | :--- | :--- |
| `abs()` | Numeric | Returns the absolute value. |
| `round()` | Numeric | Rounds a number to specified decimals. |
| `min()` / `max()` | Numeric | Finds the smallest or largest value. |
| `len()` | String | Returns the length of the string. |

---

## 6. String Indexing & Slicing
Access specific parts of a string using indices.

- **Indexing:** `text[0]` (First character)
- **Slicing:** `text[start:end:step]`
- **Reverse:** `text[::-1]`

**Example:**
```python
text = "Python"
print(text[0:2]) # Py
```

---

## 7. String Methods
Methods are functions that belong to the string class and help in text cleaning.

- `.lower()` / `.upper()`: Change case.
- `.strip()`: Remove whitespace or specific characters.
- `.replace(old, new)`: Swap substrings.
- `.split(separator)`: Break string into a list.
- `"".join(list)`: Combine list into a string.

---

## 8. F-Strings & Docstrings
### F-Strings
A modern way to format strings by embedding expressions inside `{}`.
```python
name = "Lalin"
print(f"Hello, {name}!")
```

### Docstrings
Used for documenting functions, classes, and modules.
```python
def area(l, w):
    """Calculates the area of a rectangle."""
    return l * w
```

