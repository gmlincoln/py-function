# 🐍 Python Functions: A Complete Guide for Beginners

Functions are the building blocks of clean, reusable, and organized Python code. This guide covers everything from basic syntax to advanced topics like arbitrary arguments and lambda functions.

---

## 🧠 What is a Function?

A function is a **reusable block of code** designed to perform a specific task.

### Benefits of Using Functions:
* ✅ **Avoid Repeating Code** (Don't Repeat Yourself - DRY principle)
* ✨ **Make Programs Cleaner** and more readable
* 🧩 **Organize Logic Properly** into manageable units

---

## 📍 Essential Function Concepts

### 1. Creating and Calling a Function
The basic syntax uses the `def` keyword, followed by the function name and parentheses `()`.

| Concept | Syntax/Example |
| :--- | :--- |
| **Basic Syntax** | `def function_name():` |
| **Example** | `def greet(): print("Hello Python!")` |
| **Calling** | `greet()` |

### 2. Parameters, Arguments, and Return Values

| Concept | Description | Example |
| :--- | :--- | :--- |
| **Parameters** | Pass information **into** the function. | `def greet(name): print("Hello", name)` |
| **Multiple Parameters** | Define multiple inputs separated by commas. | `def add(a, b): print(a + b)` |
| **Return Value** | Sends a value **back** from the function using the `return` keyword. | `def add(a, b): return a + b` |

> **Why use `return`?** To store the result, use it later, or build complex logic.

---

## 🛠️ Advanced Function Features

### 5. Default Parameters
If an argument is not passed when calling the function, the defined **default value** is used.

```python
def greet(name="Student"):
    print("Hello", name)

greet()          # Output: Hello Student
greet("Lincoln") # Output: Hello Lincoln
```




### 📘 Practice Questions
#### ✔ Basic
- Create a function that prints your name.  
- Write a function that takes two numbers and prints the sum.

#### ✔ Intermediate
- Create a function with default parameters.  
- Write a function that returns the largest of three numbers.  
- Use *args to add all numbers passed.  

#### ✔ Advanced
- Create a function that returns both sum and average.  
- Use **kwargs to print student details.  
- Write a lambda that squares, cubes, and doubles numbers.