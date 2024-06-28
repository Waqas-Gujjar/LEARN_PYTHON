# Variables in Python

In Python, a **variable** is a symbolic name that references a value stored in the computer's memory. Variables are dynamically typed, meaning their type is determined at runtime and can change during execution.

## Characteristics of Variables

1. **Dynamic Typing:** The type of a variable is determined at runtime.
2. **Case Sensitivity:** Variable names are case-sensitive (`Var` and `var` are different).
3. **Naming Rules:** Variable names must start with a letter (a-z, A-Z) or an underscore (_). They can include numbers, but cannot start with them. Keywords cannot be used as variable names.

## Basic Operations with Variables

### 1. Assignment

You assign a value to a variable using the `=` operator.

```python
x = 10
y = "Hello, World!"
z = 3.14
```


Certainly! Below is a README.md file explaining variables in Python with examples and common methods.

markdown
Copy code
# Variables in Python

In Python, a **variable** is a symbolic name that references a value stored in the computer's memory. Variables are dynamically typed, meaning their type is determined at runtime and can change during execution.

## Characteristics of Variables

1. **Dynamic Typing:** The type of a variable is determined at runtime.
2. **Case Sensitivity:** Variable names are case-sensitive (`Var` and `var` are different).
3. **Naming Rules:** Variable names must start with a letter (a-z, A-Z) or an underscore (_). They can include numbers, but cannot start with them. Keywords cannot be used as variable names.

## Basic Operations with Variables

### 1. Assignment

You assign a value to a variable using the `=` operator.

```python
x = 10
y = "Hello, World!"
z = 3.14
```
### 2. Multiple Assignments
You can assign values to multiple variables simultaneously.

```python
a, b, c = 1, 2, 3
```
### 3. Swapping Variables
You can swap the values of two variables in a single statement.

```python

x, y = y, x
```
### 4. Updating Variables
You can update the value of a variable based on its current value.

```python

x = 10
x = x + 5  # Now x is 15
```
### 5. Type Checking
You can check the type of a variable using the type() function.

```python

type(x)  # This will return <class 'int'>
```
## Example Usage


```python

# Assigning values to variables
name = "Alice"
age = 25
height = 5.6

# Printing variable values
print("Name:", name)
print("Age:", age)
print("Height:", height)

# Performing arithmetic operations
x = 10
y = 20
sum = x + y
print("Sum:", sum)

# Checking the type of a variable
print("Type of name:", type(name))  # <class 'str'>
print("Type of age:", type(age))    # <class 'int'>
print("Type of height:", type(height))  # <class 'float'>

# Swapping values of variables
a = 5
b = 10
a, b = b, a
print("After swapping, a:", a, "b:", b)
```

# Common Methods and Functions Associated with Variables
Depending on the type of the value stored in the variable, different methods and functions can be used. Here are some examples for common types:

## 1. For Strings
```python

name = "Alice"
print(name.upper())   # 'ALICE'
print(name.lower())   # 'alice'
print(name.replace('A', 'O'))  # 'Olice'
print(len(name))      # 5 (length of the string)
```
## 2. For Lists
```python

numbers = [1, 2, 3, 4, 5]
numbers.append(6)     # Adds 6 to the end of the list
print(numbers)        # [1, 2, 3, 4, 5, 6]
numbers.pop()         # Removes and returns the last item
print(numbers)        # [1, 2, 3, 4, 5]
print(len(numbers))   # 5 (length of the list)
```
## 3. For Dictionaries
```python

person = {"name": "Alice", "age": 25}
print(person.keys())   # dict_keys(['name', 'age'])
print(person.values()) # dict_values(['Alice', 25])
print(person.get("name"))  # 'Alice'
person.update({"height": 5.6})  # Add a new key-value pair
print(person)  # {'name': 'Alice', 'age': 25, 'height': 5.6}
```
Understanding and utilizing variables effectively is fundamental to programming in Python. They allow you to store and manipulate data, making your code flexible and dynamic.