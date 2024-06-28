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

# Variable Practice Questions

Test your understanding of variables in Python with these practice questions, categorized by difficulty levels.

## Beginner Level

1. **Simple Assignment**
   - Assign the value 42 to a variable named `answer`.
   - **Code:**
     ```python
     answer = 42
     ```

2. **Variable Types**
   - Assign the value `"Python"` to a variable `language` and the value `3.14` to a variable `pi`.
   - **Code:**
     ```python
     language = "Python"
     pi = 3.14
     ```

3. **Print Variables**
   - Create variables `name` with the value `"Alice"` and `age` with the value `30`. Print them in the format: `Name: Alice, Age: 30`.
   - **Code:**
     ```python
     name = "Alice"
     age = 30
     print(f"Name: {name}, Age: {age}")
     ```

4. **Multiple Assignments**
   - Assign the values `5`, `10`, and `15` to the variables `x`, `y`, and `z` respectively in one line.
   - **Code:**
     ```python
     x, y, z = 5, 10, 15
     ```

5. **Type Checking**
   - Create a variable `message` with the value `"Hello, World!"`. Use Python to check the type of the variable.
   - **Code:**
     ```python
     message = "Hello, World!"
     print(type(message))  # Output: <class 'str'>
     ```

## Intermediate Level

1. **Swapping Values**
   - Given two variables `a = 100` and `b = 200`, swap their values.
   - **Code:**
     ```python
     a, b = 100, 200
     a, b = b, a
     print(a, b)  # Output: 200 100
     ```

2. **Updating a Variable**
   - Create a variable `count` with the value `5`. Increment its value by `10` and print the result.
   - **Code:**
     ```python
     count = 5
     count += 10
     print(count)  # Output: 15
     ```

3. **List Manipulation**
   - Create a list `numbers` with values `[1, 2, 3, 4, 5]`. Append the value `6` to the list and print the updated list.
   - **Code:**
     ```python
     numbers = [1, 2, 3, 4, 5]
     numbers.append(6)
     print(numbers)  # Output: [1, 2, 3, 4, 5, 6]
     ```

4. **String Methods**
   - Create a variable `text` with the value `"hello world"`. Convert it to uppercase and print the result.
   - **Code:**
     ```python
     text = "hello world"
     print(text.upper())  # Output: "HELLO WORLD"
     ```

5. **Dictionary Operations**
   - Create a dictionary `student` with keys `name` and `grade`, and values `"Bob"` and `85` respectively. Add a new key `age` with the value `21`.
   - **Code:**
     ```python
     student = {"name": "Bob", "grade": 85}
     student["age"] = 21
     print(student)  # Output: {'name': 'Bob', 'grade': 85, 'age': 21}
     ```

## Advanced Level

1. **Variable Assignment in Loops**
   - Write a loop that iterates through a list `['a', 'b', 'c']` and assigns each element to a variable `letter`. Print `letter` on each iteration.
   - **Code:**
     ```python
     for letter in ['a', 'b', 'c']:
         print(letter)
     ```

2. **Chaining Assignments**
   - Assign the value `100` to three variables `x`, `y`, and `z` in a single line of code.
   - **Code:**
     ```python
     x = y = z = 100
     ```

3. **Conditional Assignment**
   - Create a variable `status` and assign it the value `"adult"` if `age` is greater than or equal to 18; otherwise, assign it `"minor"`. Assume `age` is a variable with some integer value.
   - **Code:**
     ```python
     age = 20
     status = "adult" if age >= 18 else "minor"
     print(status)  # Output: "adult"
     ```

4. **Using `isinstance()`**
   - Write a function `check_type` that takes a variable and returns whether it's a string, integer, or float.
   - **Code:**
     ```python
     def check_type(var):
         if isinstance(var, str):
             return "String"
         elif isinstance(var, int):
             return "Integer"
         elif isinstance(var, float):
             return "Float"
         else:
             return "Other"

     print(check_type("Hello"))  # Output: "String"
     print(check_type(123))      # Output: "Integer"
     print(check_type(4.56))     # Output: "Float"
     ```

5. **Complex Dictionary Manipulation**
   - Given a dictionary `data = {"a": 1, "b": 2, "c": 3}`, write a Python code to increment the value of each key by `1`.
   - **Code:**
     ```python
     data = {"a": 1, "b": 2, "c": 3}
     for key in data:
         data[key] += 1
     print(data)  # Output: {'a': 2, 'b': 3, 'c': 4}
     ```

Use these questions to practice and solidify your understanding of how to work with variables in Python at different levels of difficulty.
