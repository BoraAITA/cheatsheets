# 🐍 Python Cheatsheet

## Basic Syntax

```python
# Variables
name = "Ali"                # String
age = 25                    # Integer
height = 1.75               # Float
active = True               # Boolean
lst = [1, 2, 3]             # List
dict = {"key": "value"}     # Dict
s = {1, 2, 3}               # Set
```

## Control Structures

```python
# If/Else
if condition:
    pass
elif another_condition:
    pass
else:
    pass

# For loop
for i in range(10):
    print(i)

# While
while condition:
    break
```

## Functions

```python
# Regular function
def hello(name):
    return f"Hello {name}!"

# Lambda
add = lambda x, y: x + y

# Default parameter
def greet(name="World"):
    return f"Hello {name}!"

# *args and **kwargs
def func(*args, **kwargs):
    pass
```

## List Comprehension

```python
# Basic
squares = [x**2 for x in range(10)]

# Conditional
evens = [x for x in range(20) if x % 2 == 0]

# Nested
matrix = [[j for j in range(3)] for i in range(3)]
```

## File Operations

```python
# Reading
with open("file.txt", "r") as f:
    content = f.read()

# Writing
with open("file.txt", "w") as f:
    f.write("Hello World!")

# Line by line
with open("file.txt") as f:
    for line in f:
        print(line.strip())
```

## Error Handling

```python
try:
    result = 10 / 0
except ZeroDivisionError as e:
    print(f"Error: {e}")
except Exception as e:
    print(f"Unexpected error: {e}")
finally:
    print("Always runs")
```

## Class

```python
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age
    
    def introduce(self):
        return f"I'm {self.name}, {self.age} years old."
```

## Tips

```python
# f-string (Python 3.6+)
name = "Ali"
age = 25
print(f"Hello {name}, you are {age} years old.")

# Walrus operator (Python 3.8+)
if (n := len("hello")) > 5:
    print(f"Length: {n}")

# Unpacking
a, b, *rest = [1, 2, 3, 4, 5]
```
