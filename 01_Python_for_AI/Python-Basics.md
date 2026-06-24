# 🐍 Python Basics

## What is Python?

Python is a **high-level, interpreted, and easy-to-learn programming language**. It is one of the most popular languages in the world and is widely used in:

* Artificial Intelligence (AI)
* Machine Learning (ML)
* Data Science
* Web Development
* Automation
* Software Development

### Why is Python popular?

✅ Simple and readable syntax
✅ Beginner-friendly
✅ Large community support
✅ Huge collection of libraries
✅ Widely used in AI and Machine Learning

---

# Your First Python Program

```python
print("Hello, World!")
```

### Output

```text
Hello, World!
```

### Explanation

* `print()` is a built-in function.
* It displays the text inside the parentheses on the screen.

---

# Comments

Comments are notes written inside the code. Python ignores them during execution.

### Single-Line Comment

```python
# This is a comment
print("Hello")
```

### Multi-Line Comment

```python
"""
This is a
multi-line comment
"""
```

---

# Variables

A variable is a container that stores data.

### Example

```python
name = "Arvind"
age = 21

print(name)
print(age)
```

### Output

```text
Arvind
21
```

Think of a variable as a labeled box:

```text
name ───► "Arvind"
age  ───► 21
```

---

# Rules for Naming Variables

✅ Can contain letters, numbers, and underscores

```python
student_name = "Rahul"
age1 = 20
```

❌ Cannot start with a number

```python
1name = "Rahul"   # Invalid
```

❌ Cannot use Python keywords

```python
class = 10        # Invalid
```

---

# Data Types

A data type tells Python what kind of value is stored.

## Integer (int)

Whole numbers.

```python
age = 21
marks = 95
```

---

## Float (float)

Decimal numbers.

```python
height = 5.8
price = 99.99
```

---

## String (str)

Text enclosed in quotes.

```python
name = "Arvind"
city = 'Delhi'
```

---

## Boolean (bool)

Stores only two values:

```python
True
False
```

Example:

```python
is_student = True
is_logged_in = False
```

---

# Checking Data Type

Use `type()`.

```python
age = 21

print(type(age))
```

Output:

```text
<class 'int'>
```

---

# Taking User Input

```python
name = input("Enter your name: ")

print("Hello", name)
```

### Example

```text
Enter your name: Arvind
Hello Arvind
```

---

# Type Conversion

Input is always taken as a string.

```python
age = input("Enter age: ")
print(type(age))
```

Output:

```text
<class 'str'>
```

Convert it:

```python
age = int(input("Enter age: "))
```

### Common Conversions

```python
int("25")
float("5.5")
str(100)
bool(1)
```

---

# Operators

Operators perform operations on values.

---

## Arithmetic Operators

| Operator | Meaning        | Example |
| -------- | -------------- | ------- |
| +        | Addition       | 10 + 5  |
| -        | Subtraction    | 10 - 5  |
| *        | Multiplication | 10 * 5  |
| /        | Division       | 10 / 5  |
| //       | Floor Division | 10 // 3 |
| %        | Modulus        | 10 % 3  |
| **       | Power          | 2 ** 3  |

Example:

```python
a = 10
b = 3

print(a + b)
print(a % b)
print(a ** b)
```

---

## Comparison Operators

| Operator | Meaning               |
| -------- | --------------------- |
| ==       | Equal                 |
| !=       | Not Equal             |
| >        | Greater Than          |
| <        | Less Than             |
| >=       | Greater Than or Equal |
| <=       | Less Than or Equal    |

Example:

```python
age = 21

print(age >= 18)
```

Output:

```text
True
```

---

## Logical Operators

| Operator | Meaning                             |
| -------- | ----------------------------------- |
| and      | Both conditions must be True        |
| or       | At least one condition must be True |
| not      | Reverses the result                 |

Example:

```python
age = 21
citizen = True

print(age >= 18 and citizen)
```

Output:

```text
True
```

---

# Strings

Strings are sequences of characters.

```python
name = "Python"
```

---

## Access Characters

```python
name = "Python"

print(name[0])
print(name[1])
```

Output:

```text
P
y
```

---

## String Length

```python
name = "Python"

print(len(name))
```

Output:

```text
6
```

---

## String Methods

```python
name = "python"

print(name.upper())
print(name.lower())
print(name.capitalize())
```

Output:

```text
PYTHON
python
Python
```

---

# Lists

Lists store multiple values.

```python
fruits = ["Apple", "Banana", "Mango"]

print(fruits)
```

Output:

```text
['Apple', 'Banana', 'Mango']
```

---

## Access Elements

```python
print(fruits[0])
```

Output:

```text
Apple
```

---

## Add Items

```python
fruits.append("Orange")
```

---

## Remove Items

```python
fruits.remove("Banana")
```

---

# Tuples

Tuples are ordered and cannot be changed.

```python
colors = ("Red", "Blue", "Green")
```

---

# Sets

Sets store unique values.

```python
numbers = {1, 2, 3, 4}
```

Duplicate values are removed automatically.

---

# Dictionaries

Dictionaries store data in key-value pairs.

```python
student = {
    "name": "Arvind",
    "age": 21,
    "course": "AIML"
}

print(student["name"])
```

Output:

```text
Arvind
```

---

# Summary of Data Structures

| Data Structure | Ordered | Mutable | Allows Duplicates |
| -------------- | ------- | ------- | ----------------- |
| List           | Yes     | Yes     | Yes               |
| Tuple          | Yes     | No      | Yes               |
| Set            | No      | Yes     | No                |
| Dictionary     | Yes     | Yes     | Keys: No          |

---

# Indentation

Python uses indentation to define blocks of code.

Correct:

```python
age = 20

if age >= 18:
    print("Adult")
```

Incorrect:

```python
age = 20

if age >= 18:
print("Adult")
```

This gives an error.

---

# Keywords

Keywords are reserved words in Python.

Examples:

```text
if
else
for
while
class
def
True
False
None
return
```

You cannot use them as variable names.

---

# Python in AI and Machine Learning

Python is the backbone of modern AI.

Examples:

```python
import pandas as pd
import numpy as np
from sklearn.linear_model import LinearRegression
import matplotlib.pyplot as plt
```

Almost every AI project starts with Python and its libraries.

---

# Key Takeaways

* Python is simple, powerful, and beginner-friendly.
* Variables store data.
* Data types define what kind of data is stored.
* Operators perform calculations and comparisons.
* Strings store text.
* Lists, tuples, sets, and dictionaries store collections of data.
* Indentation is extremely important in Python.
* Python is the most widely used language in Artificial Intelligence and Machine Learning.

---

> **"Learn Python fundamentals well. Every Machine Learning model, data pipeline, and AI application you build later will depend on these basics."**
