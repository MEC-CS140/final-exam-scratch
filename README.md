# CS140: Computer Science Seminar - Python Starter Template

Welcome to this Python starter template 🚀 to supercharge your Python skills! We will use this template for class notes. 
This README covers practical tips and sample code snippets for variables, strings, integers, booleans, functions, and logical operations.

## Table of Contents

- [Variables](#variables)
- [Strings](#strings)
- [Integers](#integers)
- [Booleans](#booleans)
- [Functions](#functions)
- [If Statements](#if-statements)

## Variables

Variables store data values. A variable is created the moment you first assign a value to it.

### Tips:
- Use meaningful variable names to make your code more readable.
- Python is dynamically typed, which means you can reassign variables to different data types.

```python
x = 5
x = "Hello"  # Now x is of type str
```

## Strings

Strings in Python represents text. Strings are enclosed in double quotes `""`.

### Tips:
- Use the `+` operator to concatenate strings directly.
- For better performance and readability, especially with multiple strings, consider using the `.join()` method.

# Using the + operator
```python
greeting = "Hello"
name = "Alice"
sentence = greeting + ", " + name + "!"
print(sentence)  # Outputs 'Hello, Alice!'
```

# Using the join method for multiple parts
```python
words = ["Hello", "world", "from", "Python"]
sentence = " ".join(words)
print(sentence)  # Outputs 'Hello world from Python'
```

You can also:
- Trim spaces with strip()
- Find substrings with find() or in
- Replace parts of strings with replace()
- Here are some quick examples to get you started:

```python
phrase = "   Hello, world!   "
trimmed = phrase.strip()
print(trimmed)  # Outputs 'Hello, world!'
```
# Checking for a substring
```python
contains_world = "world" in trimmed
print(contains_world)  # Outputs True
```
# Replacing text
```python
updated_phrase = trimmed.replace("Hello", "Goodbye")
print(updated_phrase)  # Outputs 'Goodbye, world!'
```

## Integers

In Python, an integer is a whole number, positive or negative, without decimals of unlimited length.

# Creating an integer

```python
my_int = 10
print(my_int)  # Outputs 10
```

# Converting an integer to a string
```python
my_str = str(my_int)
print(my_str)  # Outputs '10'
```
# Converting a string to an integer

```python
new_int = int(my_str)
print(new_int)  # Outputs 10
```

## Booleans

Booleans represent one of two values: `True` or `False`. Boolean expressions are often used in conditional statements and loops.

### Tips:
- Use Boolean expressions directly in conditions without explicit comparison operators.

```python
flag = True
if flag:
    print("Flag is True")
```

## Functions

Functions in Python are defined using the `def` keyword. They organize code into manageable blocks, making your programs easier to write and read.

### Tips
- Keep it short and sweet: Aim for functions that perform a single task. This makes them easier to test, understand, and reuse.
- Use descriptive names: Function names should be descriptive enough to convey their purpose. For example, calculate_total() is more informative than func1().
- Limit the number of arguments: Ideally, functions should have a few arguments. If you find yourself needing more, consider whether your function is doing too much or if you should use a class to encapsulate the data.

# A simple function with a return statement
```python
def get_message():
    return "Hello, world!"

message = get_message()
print(message)  # Outputs 'Hello, world!'
```

# A function with arguments but no return value
```python
def print_sum(x, y):
    print("The sum is:", x + y)

print_sum(5, 3)  # Outputs 'The sum is: 8'
```
# A function with arguments and a return value
```python
def multiply_numbers(a, b):
    return a * b

result = multiply_numbers(4, 3)
print(result)  # Outputs 12
```


## If Statements

### Tips:
- Use clear conditions: Make your conditions straightforward and easy to understand.
- Avoid unnecessary nesting: Where possible, keep your if statements flat. Deeply nested if statements can make your code hard to read and maintain.
- Use elif for multiple conditions: If you have several conditions that are mutually exclusive, elif can be a cleaner alternative to multiple if statements.
- Combine conditions with logical operators: Use and, or, and not to combine conditions, making complex decisions easier to manage.

# Simple if statements
```python

age = 18
if age >= 18:
    print("You are an adult.")

x = 10
if x > 5 and x < 15:
    print("x is between 5 and 15")

if not x > 20:
    print("x is not greater than 20")
```

# Using if-else statement

```python
temperature = 20
if temperature > 25:
    print("It's warm outside.")
else:
    print("It's not warm outside.")
```


