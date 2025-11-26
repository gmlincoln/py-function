Python Function – Complete Guide for Beginners
🧠 What is a Function?

A function is a reusable block of code that performs a specific task.
Functions help you:

avoid repeating code

make programs cleaner

organize logic properly

📍 1. Creating a Function
✔ Basic Syntax
def function_name():
    # code block

✔ Example
def greet():
    print("Hello Python!")

✔ Calling a function
greet()

📍 2. Function with Parameters

Parameters allow you to pass information into a function.

def greet(name):
    print("Hello", name)

greet("Rafi")

📍 3. Function with Multiple Parameters
def add(a, b):
    print(a + b)

add(10, 20)

📍 4. Function with Return Value

return sends a value back from the function.

def add(a, b):
    return a + b

result = add(5, 7)
print(result)    # 12

✔ Why use return?

To store the result

To use the result later

To build more complex logic

📍 5. Default Parameters

If no value is passed, default is used.

def greet(name="Student"):
    print("Hello", name)

greet()          # Hello Student
greet("Lincoln") # Hello Lincoln

📍 6. Keyword Arguments (Flexible)
def info(name, age):
    print(name, age)

info(age=22, name="Rafi")

📍 7. Arbitrary Arguments (*args)

Used when you don’t know how many arguments will come.

def total(*numbers):
    print(sum(numbers))

total(1, 2, 3, 4)   # 10


*args collects values as a tuple

📍 8. Arbitrary Keyword Arguments (**kwargs)

Used for unknown number of key–value arguments.

def details(**info):
    print(info)

details(name="Rafi", age=22, city="Dhaka")


**kwargs collects values as a dictionary

📍 9. Docstring (Function Documentation)
def add(a, b):
    """This function returns the sum of two numbers."""
    return a + b

print(add.__doc__)

📍 10. The pass Statement (Empty Function)
def temp():
    pass


Used as a placeholder.

📍 11. Nested Functions (Function inside function)
def outer():
    print("Outer function")

    def inner():
        print("Inner function")

    inner()

outer()

📍 12. Lambda Functions (Single-line function)

Anonymous, one-line function.

square = lambda x: x * x
print(square(5))

📍 13. Function with Multiple Return Values
def person():
    return "Rafi", 22, "Dhaka"

name, age, city = person()
print(name, age, city)

📍 14. Global and Local Variables
✔ Local variable → inside function
✔ Global variable → outside function
x = 10  # global

def show():
    y = 5  # local
    print(x, y)

show()

📍 15. Global Keyword

To modify global variable inside a function:

x = 10

def update():
    global x
    x = 20

update()
print(x)   # 20

📍 16. Function Use Cases
✔ 1. Avoid repeating code
def welcome():
    print("Welcome to the system!")

for _ in range(5):
    welcome()

✔ 2. Data processing
def average(numbers):
    return sum(numbers)/len(numbers)

✔ 3. Input validation
```python
def is_valid_age(age):
    return age > 0
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