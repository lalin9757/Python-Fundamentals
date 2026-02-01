# Python Fundamentals for Data Science & Machine Learning (Part 01)

This repository contains the foundational concepts of **Python Programming**, specifically designed for beginners entering the fields of Data Science and Machine Learning. It covers everything from setting up your environment to understanding complex data structures and mutability.

## 📋 Table of Contents
- [1. Introduction to Python](#1-introduction-to-python)
- [2. Google Colab & Jupyter Notebook](#2-google-colab--jupyter-notebook)
- [3. Variables & Naming Conventions](#3-variables--naming-conventions)
- [4. Python Data Types](#4-python-data-types)
- [5. Iterables & Mutability](#5-iterables--mutability)
- [6. List vs. Tuples](#6-list-vs-tuples)
- [🚀 Getting Started](#-getting-started)

---

## 1. Introduction to Python
Python is a high-level, interpreted, and general-purpose programming language known for its simplicity and readability.

**Why Python for DS & ML?**
- **Rich Ecosystem:** Libraries like NumPy, Pandas, Scikit-learn, and TensorFlow.
- **Community Support:** Large global community for troubleshooting and resources.
- **Prototyping:** Excellent for moving from ideas to production-level code quickly.

---

## 2. Google Colab & Jupyter Notebook
Interactive environments are essential for data science workflows.

- **Google Colab:** A cloud-based platform that requires no setup and provides free access to GPUs.
- **Jupyter Notebook:** An open-source web app for creating documents with live code and visualizations.

**Pro Tip:** Use `Shift + Enter` to run a cell and move to the next one.

---

## 3. Variables & Naming Conventions
Variables are containers for storing data values.

| Concept | Description |
| :--- | :--- |
| **Assigning** | Use the `=` operator (e.g., `x = 5`). |
| **Overwriting** | Reassigning a new value to an existing variable. |
| **Deleting** | Use the `del` keyword to remove a variable from memory. |

**Example: Assigning and Overwriting**
```python
name = "Alice"  # Assigning
print("Name:", name)

name = "Bob"  # Overwriting
print("Updated Name:", name)

user_age = 25  # Descriptive and snake_case
print("User Age:", user_age)
```

---

## 4. Python Data Types
Python has several built-in data types that are fundamental to data manipulation.

| Data Type | Example | Description |
| :--- | :--- | :--- |
| **Integer** | `age = 25` | Whole numbers. |
| **Float** | `height = 5.9` | Decimal numbers. |
| **String** | `"Hello"` | Sequence of characters. |
| **Boolean** | `True / False` | Logical values. |
| **List** | `[1, 2, 3]` | Ordered, mutable collection. |
| **Tuple** | `(10, 20)` | Ordered, immutable collection. |
| **Dictionary** | `{"id": 1}` | Key-value pairs. |

**Code Examples for Data Types:**
```python
# Numeric Types
age = 25          # int
height = 5.9      # float
print(f"Age: {age}, Type: {type(age)}")
print(f"Height: {height}, Type: {type(height)}")

# Strings
name = "Rossi"
greeting = 'Hello, ' + name
print(greeting) # Output: Hello, Rossi

# Lists (Mutable)
fruits = ["apple", "banana", "cherry"]
fruits.append("orange")  # Add an item
print("Fruits:", fruits) # Output: ['apple', 'banana', 'cherry', 'orange']

# Tuples (Immutable)
coordinates = (10.0, 20.0)
print("X-coordinate:", coordinates[0]) # Output: 10.0

# Dictionaries
person = {"name": "Nayeem", "age": 25}
print("Name:", person["name"])  # Access by key
person["age"] = 26  # Update value
print("Updated Age:", person["age"]) # Output: 26
```

---

## 5. Iterables & Mutability
Understanding how Python handles data changes is crucial for debugging.

### Mutability
- **Mutable:** Can be changed after creation (e.g., Lists, Dictionaries, Sets).
- **Immutable:** Cannot be changed after creation (e.g., Strings, Tuples, Integers).

**Example: Mutability**
```python
# List (Mutable)
colors = ["red", "green", "blue"]
colors[0] = "yellow"
print("Updated Colors:", colors) # Output: ['yellow', 'green', 'blue']

# Tuple (Immutable) - This would raise an error if uncommented
# rgb = ("red", "green", "blue")
# rgb[0] = "yellow"
```

### Iterables
Objects that can be looped over (e.g., using a `for` loop). This includes Sequences (Lists, Tuples), Mappings (Dictionaries), and Sets.

---

## 6. List vs. Tuples
While both store collections of items, they serve different purposes:

- **Lists `[]`:** Use when you need a collection that can grow or change (e.g., a list of users).
- **Tuples `()`:** Use for fixed data that shouldn't change (e.g., GPS coordinates or RGB values). Tuples are generally faster than lists.

---

## 🚀 Getting Started
To run the code in this repository:
1. Open the `.ipynb` file in **Google Colab** or **Jupyter Notebook**.
2. Follow the session outline to understand the basics.
3. Experiment by modifying the variables and running the cells.

---
*This documentation serves as a foundational guide for anyone starting their journey in Python for Data Science.*
