# 🏛️ Object-Oriented Programming (OOP) in Python

## What is Object-Oriented Programming (OOP)?

Object-Oriented Programming (OOP) is a programming style that organizes code into **objects**.

Instead of writing everything in one place, OOP groups **data** and the **functions that work on that data** together.

Think of OOP as describing real-world objects in code.

For example:

* 🚗 Car
* 👨 Student
* 🏦 Bank Account
* 📱 Mobile Phone

Each object has:

* **Properties (Data)** → What it has
* **Behaviors (Functions)** → What it can do

---

# Real Life Example

Imagine a **Car**.

A car has:

### Properties (Attributes)

* Brand
* Color
* Speed
* Fuel

### Behaviors (Methods)

* Start
* Stop
* Accelerate
* Brake

We can represent the same thing in Python.

---

# What is a Class?

A **Class** is a blueprint or template for creating objects.

Think of it like an architectural blueprint.

Example:

Blueprint of a House
↓

Many houses can be built from it.

Similarly,

Class
↓

Many objects can be created from it.

---

## Syntax

```python
class Student:
    pass
```

Here,

* `class` is a keyword.
* `Student` is the class name.

Currently, this class does nothing because of the `pass` keyword.

---

# What is an Object?

An **Object** is a real instance of a class.

Example:

Class

```text
Student
```

Objects

```text
Arvind
Rahul
Priya
```

All three are students, but each has different information.

---

## Creating an Object

```python
class Student:
    pass

student1 = Student()
student2 = Student()
```

Here,

* `Student()` creates an object.
* `student1` and `student2` are different objects.

---

# Understanding with an Example

Imagine a class called **Dog**.

Every dog has:

* Name
* Age

Let's create it.

```python
class Dog:

    def __init__(self, name, age):
        self.name = name
        self.age = age
```

Now create objects.

```python
dog1 = Dog("Tommy", 3)
dog2 = Dog("Bruno", 5)
```

---

# What is `__init__()`?

This is called the **Constructor**.

It automatically runs whenever an object is created.

Think of it as the object's setup function.

Example:

```python
student = Student()
```

Python automatically calls

```python
__init__()
```

---

# Understanding `self`

Beginners usually find `self` confusing.

Don't worry.

Think of `self` as **"this object"**.

Example:

```python
class Student:

    def __init__(self, name):
        self.name = name
```

Suppose

```python
student1 = Student("Arvind")
```

Python internally does something like

```text
student1.name = "Arvind"
```

Now,

```python
print(student1.name)
```

Output

```text
Arvind
```

So,

`self` simply refers to the current object.

---

# Attributes

Attributes are variables that belong to an object.

Example

```python
class Student:

    def __init__(self, name, age):
        self.name = name
        self.age = age
```

Here,

* name
* age

are attributes.

---

# Methods

Methods are functions inside a class.

Example

```python
class Student:

    def __init__(self, name):
        self.name = name

    def introduce(self):
        print("My name is", self.name)
```

Create object

```python
student = Student("Arvind")

student.introduce()
```

Output

```text
My name is Arvind
```

---

# Complete Example

```python
class Student:

    def __init__(self, name, age):
        self.name = name
        self.age = age

    def display(self):
        print("Name :", self.name)
        print("Age  :", self.age)


student1 = Student("Arvind",21)

student1.display()
```

Output

```text
Name : Arvind
Age  : 21
```

---

# Four Pillars of OOP

These are the four main concepts of Object-Oriented Programming.

```text
1. Encapsulation
2. Inheritance
3. Polymorphism
4. Abstraction
```

Let's understand each one.

---

# 1. Encapsulation

### Meaning

Keeping **data and functions together** inside one class.

Example

Think of a smartphone.

You can use it.

But you cannot directly access the internal circuits.

Everything is safely packed together.

In Python

```python
class Student:

    def __init__(self,name):
        self.name = name
```

Both data and functions belong to the Student class.

---

# 2. Inheritance

Inheritance means one class can use the properties and methods of another class.

Real-life example

```text
Animal
   │
   ├── Dog
   ├── Cat
   └── Lion
```

All animals can eat.

Dogs don't need to rewrite the eating behavior.

Example

```python
class Animal:

    def speak(self):
        print("Animal speaks")


class Dog(Animal):
    pass


dog = Dog()

dog.speak()
```

Output

```text
Animal speaks
```

Dog inherited the method from Animal.

---

# 3. Polymorphism

"Poly" means many.

"Morphism" means forms.

The same method can behave differently depending on the object.

Example

```python
class Dog:

    def sound(self):
        print("Bark")


class Cat:

    def sound(self):
        print("Meow")
```

Same method

```python
sound()
```

Different outputs.

---

# 4. Abstraction

Abstraction means hiding unnecessary details from the user.

Example

You drive a car.

You only use

* Steering
* Brake
* Accelerator

You don't need to know how the engine works.

Similarly,

Python lets us hide complex implementation details.

---

# Why Use OOP?

Without OOP

```text
Everything is mixed together.
Large programs become difficult to manage.
```

With OOP

✅ Organized code

✅ Reusable code

✅ Easy to maintain

✅ Easy to debug

✅ Better for large projects

---

# OOP in AI and Machine Learning

Almost every AI library uses OOP.

Example

```python
from sklearn.linear_model import LinearRegression

model = LinearRegression()

model.fit(X_train, y_train)

predictions = model.predict(X_test)
```

Here,

`LinearRegression` is a class.

`model` is an object.

`fit()` and `predict()` are methods.

Similarly,

PyTorch

```python
model.train()
model.eval()
```

TensorFlow

```python
model.compile()
model.fit()
```

Everything is based on OOP.

---

# Summary

| Concept                  | Meaning                                  |
| ------------------------ | ---------------------------------------- |
| Class                    | Blueprint for creating objects           |
| Object                   | Instance of a class                      |
| Constructor (`__init__`) | Initializes an object when it is created |
| self                     | Refers to the current object             |
| Attribute                | Variable belonging to an object          |
| Method                   | Function inside a class                  |
| Encapsulation            | Keep data and methods together           |
| Inheritance              | Reuse code from another class            |
| Polymorphism             | Same method, different behavior          |
| Abstraction              | Hide unnecessary implementation details  |

---

# Key Takeaways

* OOP helps organize programs using **classes** and **objects**.
* A **class** is a blueprint, while an **object** is a real instance created from that blueprint.
* The **constructor (`__init__`)** initializes object data automatically.
* **`self`** refers to the current object.
* OOP is built on four pillars:

  * Encapsulation
  * Inheritance
  * Polymorphism
  * Abstraction
* Modern AI libraries such as **Scikit-learn, TensorFlow, PyTorch, LangChain, and Hugging Face** heavily rely on OOP.

---

> **💡 Tip:** If you're new to OOP, don't try to memorize definitions. Create simple classes like `Student`, `Car`, `Book`, or `BankAccount`, make multiple objects from them, and experiment. Once you can build these on your own, the core concepts of OOP will become much easier to understand.
