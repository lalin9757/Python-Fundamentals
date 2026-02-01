# Python Fundamentals - Session 03

This repository contains a Jupyter Notebook (`Seassion03.ipynb`) that covers essential Python programming concepts, ranging from basic function definitions to more advanced topics like list comprehensions and matrix operations.

## Table of Contents
1. [User-Defined Functions](#user-defined-functions)
2. [Functions with Parameters](#functions-with-parameters)
3. [Nested Functions](#nested-functions)
4. [Iteration (Loops)](#iteration-loops)
5. [Iterating Over Dictionaries](#iterating-over-dictionaries)
6. [List Comprehension](#list-comprehension)
7. [Error Handling](#error-handling)
8. [Lambda Functions](#lambda-functions)
9. [Matrix Operations](#matrix-operations)
10. [How to Run](#how-to-run)

---

## User-Defined Functions
Learn how to define and call basic functions in Python to reuse code blocks.

```python
# Defining and calling a function
def greet():
    print("Hello World!!")

greet()
```

## Functions with Parameters
Functions can accept arguments to perform operations on dynamic data.

```python
def greet_user(name):
    print(f"Hello, {name}")

greet_user("Lalin")

# Example: Palindrome Checker
def isPalindrome(word):
    return word == word[::-1]

word = "wow"
if isPalindrome(word):
    print("Yes, It's Palindrome.")
```

## Nested Functions
Python allows defining functions inside other functions, useful for encapsulation.

```python
def outer_function():
    print("This is outer function.")
    def inner_function():
        print("This is inner function.")
    inner_function()

outer_function()
```

## Iteration (Loops)
Explore the use of `for` and `while` loops for repeating tasks.

```python
# For loop
fruits = ["apple", "banana", "orange"]
for f in fruits:
    print(f)

# While loop
count = 0
while count < 3:
    print("Count:", count)
    count += 1
```

## Iterating Over Dictionaries
Efficiently access keys and values within a dictionary.

```python
person = {"name": "lalin", "age": 24, "is_student": True}

for key, value in person.items():
    print(f"Key: {key}, Value: {value}")
```

## List Comprehension
A concise way to create and transform lists.

```python
num = [1, 2, 3, 4, 5]
squares = [x ** 2 for x in num]
print(squares) # Output: [1, 4, 9, 16, 25]

# Filtering even numbers
even = [n for n in num if n % 2 == 0]
print(even) # Output: [2, 4]
```

## Error Handling
Use `try` and `except` blocks to handle potential runtime errors gracefully.

```python
try:
    num = int(input("Enter a number: "))
    print("You entered:", num)
except ValueError:
    print("Invalid input! Please enter a valid number.")
```

## Lambda Functions
Anonymous functions for quick, one-line operations, often used with `map()`.

```python
# Double a number
double = lambda x: x * 2
print("Double of 5 is:", double(5))

# Using with map()
num = [1, 2, 3, 4, 5]
doubled_num = list(map(lambda x: x * 2, num))
```

## Matrix Operations
Working with nested lists to represent and access 2D data structures.

```python
matrix = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
]
# Accessing element at row 2, column 3
print("Element:", matrix[1][2]) # Output: 6
```

## How to Run
1. Ensure you have Python and Jupyter Notebook/Lab installed.
2. Clone this repository.
3. Open `Seassion03.ipynb` in your Jupyter environment.
4. Run the cells sequentially to see the output.
