# Python Fundamentals for Data Science & Machine Learning

Welcome to the **Python Fundamentals for Data Science & Machine Learning** course. This repository contains the first session's materials, including detailed explanations and examples of Python basics, designed for beginners and intermediate learners.

---

## Session Outline

* Introduction to Python
* Google Colab and Jupyter Notebook Overview
* Variables: Assignment, Overwriting, Naming Conventions
* Python Data Types: Numeric, Strings, Boolean, List, Dictionary, Tuple, Set, None
* Iterables & Mutability: List vs Tuple

---

## 1. Introduction to Python

### What is Python?

* Python is a **high-level, interpreted, general-purpose programming language**.
* Known for its **simplicity and readability**, making it ideal for beginners.
* Widely used in **Data Science, Machine Learning, Web Development, Web Scraping, Automation**, and more.

### Why Python for Data Science and Machine Learning?

* **Rich ecosystem of libraries**: NumPy, Pandas, SciPy, Matplotlib, Plotly, Statsmodels, Scikit-learn, TensorFlow.
* **Easy to learn and use**, with a large community for support.
* **Efficient for prototyping and production-level code**.

---

## 2. Introduction to Google Colab & Jupyter Notebook

**Google Colab** is a free cloud service that allows you to write and execute Python code in your browser.

**Advantages:**

* No installation required.
* Free access to GPU for machine learning tasks.
* Easy sharing and collaboration.

**Jupyter Notebook** is a local or server-based notebook environment for Python development.

**Features:**

* Combine code, text, and visualizations in one file.
* Interactive execution of Python code.
* Support for Markdown formatting for documentation.

---

## 3. Variables in Python

### Assigning Variables

```python
x = 10  # integer variable
name = "Lalin"  # string variable
is_active = True  # boolean variable
```

### Overwriting Variables

```python
x = 5
x = x + 10  # x is now 15
```

### Naming Conventions

* Use **letters, numbers, and underscores**
* Cannot start with a number
* Example: `first_name`, `total_score`, `is_valid`

---

## 4. Python Data Types

### Numeric Types

```python
int_var = 10
float_var = 3.14
complex_var = 2 + 3j
```

### String

```python
text = "Hello, Python!"
print(text.upper())  # HELLO, PYTHON!
```

### Boolean

```python
is_true = True
is_false = False
```

### List

```python
my_list = [1, 2, 3, "Python"]
my_list.append(4)  # [1, 2, 3, 'Python', 4]
```

### Tuple

```python
my_tuple = (1, 2, 3)
# Immutable: cannot change values
```

### Dictionary

```python
my_dict = {"name": "Lalin", "age": 25}
print(my_dict['name'])  # Lalin
```

### Set

```python
my_set = {1, 2, 3, 3}
print(my_set)  # {1, 2, 3}
```

### None

```python
value = None
```

---

## 5. Iterables & Mutability

* **List**: Mutable, ordered collection
* **Tuple**: Immutable, ordered collection
* **Set**: Mutable, unordered collection
* **Dictionary**: Mutable, unordered key-value pairs

**Example:**

```python
my_list = [1, 2, 3]
my_tuple = (1, 2, 3)

# List can be updated
my_list[0] = 10

# Tuple cannot be updated
# my_tuple[0] = 10  # This will raise an error
```

---

This README serves as a reference for Python fundamentals in the context of Data Science and Machine Learning. For hands-on exercises and examples, please check the notebooks in this repository.

---

## Thank You!


