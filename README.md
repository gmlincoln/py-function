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

| Concept          | Syntax/Example                        |
| :--------------- | :------------------------------------ |
| **Basic Syntax** | `def function_name():`                |
| **Example**      | `def greet(): print("Hello Python!")` |
| **Calling**      | `greet()`                             |

### 2. Parameters, Arguments, and Return Values

| Concept                 | Description                                                          | Example                                 |
| :---------------------- | :------------------------------------------------------------------- | :-------------------------------------- |
| **Parameters**          | Pass information **into** the function.                              | `def greet(name): print("Hello", name)` |
| **Multiple Parameters** | Define multiple inputs separated by commas.                          | `def add(a, b): print(a + b)`           |
| **Return Value**        | Sends a value **back** from the function using the `return` keyword. | `def add(a, b): return a + b`           |

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

### 6. Keyword Arguments (Flexible Calling)
Arguments can be passed by their parameter name, allowing you to pass them in any order.

```python
def info(name, age):
    print(name, age)

info(age=22, name="Lincoln") # Order doesn't matter
```
### 7. Arbitrary Arguments (*args)
Used when you don't know the exact number of non-keyword arguments that will be passed.
*args collects all passed positional values as a tuple.

```python
def total(*numbers):
    print(sum(numbers))

total(1, 2, 3, 4) # Output: 10

```
### 8. Arbitrary Keyword Arguments (**kwargs)
Used for an unknown number of key-value arguments.

**kwargs collects all passed keyword arguments as a dictionary.

```python 
def details(**info):
    print(info)

details(name="Lincoln", age=22, city="Dhaka")
# Output: {'name': 'Lincoln', 'age': 22, 'city': 'Dhaka'}

```


## 📑 Documentation and Structure
### 9. Docstring (Function Documentation)
A string literal used to document a function, placed immediately after the function definition. Accessible via function_name.__doc__.

```python 
def add(a, b):
    """This function returns the sum of two numbers."""
    return a + b

```
### 10. The pass Statement (Empty Function)
Used as a placeholder when a function definition is required, but you haven't written the code block yet.

```python 
def temp():
    pass
```

### 11. Nested Functions (Function inside Function)
A function defined within another function. The inner function is typically only accessible from within the outer function.

```python 

def outer():
    print("Outer function")
    def inner():
        print("Inner function")
    inner()
outer()

```

### 12. Lambda Functions (Single-line Function)
Also known as anonymous functions. They are restricted to a single expression and are defined using the lambda keyword.

```python 
# Syntax: lambda arguments: expression
square = lambda x: x * x
print(square(5)) # Output: 25

```

### 13. Function with Multiple Return Values
A function can return multiple values, which are automatically packed into a tuple.

```python 
def person():
    return "Lincoln", 22, "Dhaka"

name, age, city = person()
print(name, age, city) # Output: Lincoln 22 Dhaka

```

## 🌐 Scope and Variables
### 14. Global and Local Variables
- Local variable → Defined inside a function (only exists within the function).  
- Global variable → Defined outside a function (accessible everywhere).

```python 
x = 10  # Global
def show():
    y = 5  # Local
    print(x, y)
```


### 15. The global Keyword
Used to modify a global variable from inside a function.

```python 
x = 10

def update_x():
    global x # Declares intent to modify the global x
    x = 20

update_x()
print(x) # Output: 20

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