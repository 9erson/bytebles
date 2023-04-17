# Lesson 4: Data Types and Expressions - A Deep Dive

## Introduction

In this lesson, we will **build upon** the concepts covered in the first three lessons and **dive deeper** into Python data types, built-in functions, and type conversion. We'll also introduce **two engaging projects**: a simple calculator and an amusement park ride eligibility checker.

We will **review** the following concepts from previous lessons:

1. Python data types: strings, integers, floats, and bools.
2. Displaying text on the screen using the `print` function.
3. Getting user input using the `input` function.
4. Using variables to store values.
5. Performing arithmetic operations.
6. Making decisions with `if`, `elif`, and `else` statements.

By the end of this lesson, you will have a **solid understanding** of Python's data types, built-in functions, and practical applications. Get ready to explore the exciting world of Python programming!

# Concepts

## Data Types

### Strings

Strings represent text and are surrounded by **single** or **double** quotes.

```python
string1 = 'Hello, World!'
string2 = "Python is great."
```

If a string contains **double** quotes, you can **surround** the string with **single** quotes:

```python
string1 = 'She said, "Hello, World!"'
```

If a string contains **single** quotes, you can **surround** the string with **double** quotes:

```python
string2 = "It's a wonderful day!"
```

If a string contains **both** single and double quotes, you can use **escape characters** to include the quotes within the string. The escape character is a **backslash** (`\`) followed by the quote you want to include:

```python
string3 = 'She said, "It\'s a wonderful day!"'
string4 = "She said, \"It's a wonderful day!\""
```

#### Reasons to use strings:

- When working with **textual** data, such as names, addresses, or any other textual content.
- To **store** and **manipulate** sequences of characters, like parsing and formatting text.

### Integers

- Integers are **whole** numbers **without** decimal points and are **not** surrounded by quotes.

- Integers can be **positive**, **negative**, or **zero**.
- Integers support **arithmetic operations** like addition, subtraction, multiplication, etc.

#### Examples:

```python
int1 = 42
int2 = -7
int3 = 0
int4 = 2 + 3
```

#### Reasons to use integers:

- When working with countable or discrete data, like the number of items in a list or the age of a person.
- To represent states or options in a program, like encoding days of the week as integers.

### Floats

- Floats are numbers **with decimal points** and are **not** surrounded by quotes.

- Floats can be **positive**, **negative**, or **zero**.
- Floats support **arithmetic operations** like addition, subtraction, multiplication, etc.
- Floats have **limited** precision and can have **rounding errors** when performing arithmetic operations.

#### Examples:

```python
float1 = 3.14
float2 = -0.56
float3 = 42.0
float4 = 9/2
```

#### Reasons to use floats:

- When working with **continuous** or **fractional** data, like measurements or currency.
- To represent **ratios** or **proportions** in a program, like calculating a percentage.

### Bools

- Bools, short for boolean, can either be `True` or `False` and are **not** surrounded by quotes.

- Bools are used to represent **truth values** (True or False) in **logical expressions**.
- Bools can be the result of **comparisons** (>, <, ==, !=) and **logical operations** (and, or, not).

#### Examples:

```python
bool1 = True
bool2 = False
bool3 = 5 > 3 and 5 < 10 # True, because 5 is greater than 3 and less than 10

is_signed_in = True
```

#### Reasons to use bools:

- When working with **conditions**, like controlling the flow of a program with `if`, `elif`, and `else` statements.
- To represent binary **states** or **options** in a program, like a switch being on or off.
- In **loops**, which we will cover in a future lesson.

## Boolean Expressions

1. Evaluate to `True` or `False`.
2. Use **comparison operators** (>, <, <=, >=, ==, !=) and **logical operators** (and, or, not).
3. **Parentheses** can be used to **override** the order of operations.

### Examples

```python
comparison = 5 > 3 # True because 5 is greater than 3
logical = (5 > 3) and (2 < 4) # True because both conditions are true
```

## Arithmetic Operators

1. Used with **integers** and **floats** (+, -, *, /, **, %).
2. **Evaluate** to integers or floats.
3. **Parentheses** can be used to **override** the order of operations.

### Examples

```python
addition = 5 + 3 # Addition: 8
subtraction = 5 - 3 # Subtraction: 2
multiplication = 5 * 3 # Multiplication: 15
division = 5 / 3 # Division: 1.6666666666666667 (float)
exponentiation = 5 ** 3 # Exponentiation: 125
modulo = 5 % 3 # Modulo (remainder): 2
```

## Functions

A **function** is a reusable block of code that performs a specific task. Functions help to **modularize** and **organize** your code, making it more **readable** and **maintainable**. Functions can take input values (called **parameters**) and **return** a value as output.

**Built-in functions** are **pre-defined functions** in Python that you can use to perform various **calculations**, **transformations**, and **actions**. These functions are part of the **core** Python language and are available **without** importing any additional modules.

There are **two** main components of a function: **parameters** and **return** values.

Functions can accept input values called **parameters**. Parameters are **passed** to the function when it's called and are **used** by the function to perform **calculations** or **actions**.

```python
greeting = "Hello World!"
print(greeting) # greeting is a parameter for the print function

name = "Alice"
print("Hello", name) # "Hello" and name are both parameters for the print function
```

Functions can **return** a value as output. The return value of a function can be **stored** in a **variable**, which can then be used for other **calculations**, **transformations**, or **displaying** on the screen. If a function **doesn't** return a value, it's considered to have a return value of `None`.

```python
name = input("What is your name?" ) # The input function returns the user's input as a string data type. The value is stored in the variable name.
name_length = len(name) # name is a parameter for the len function. The len function returns an integer that represents the length of name.
print(name) # That value is then displayed on the screen.
print(name_length)
```

## Type Casting

**Type Casting** is needed in certain situations when you need to **change** the data type of a variable, for example, converting a string to an integer or float, or an integer or float to a string.

### Examples

```python
string_num = input("Enter a number") # E.g. 42. This will be stored as a string. i.e. '42'
int_num = int(string_num) # Convert string to int: 42
float_num = float(string_num) # Convert string to float: 42.0
str_num = str(int_num) # Convert int to string: "42"
bool_num = bool(1) # Convert int to bool: True
bool_num = bool(0) # Convert int to bool: False
```

## Casting to Bool

When converting strings, integers and floats to bool, a value of **0**, **0.0**, or an **empty string** will evaluate to **False**, while any non-zero number or **non-empty string** will evaluate to **True**.

### Examples

#### General:

```python
bool_zero = bool(0) # False, because 0 evaluates to False
bool_non_zero = bool(42) # True, because any non-zero integer evaluates to True
```

#### Checking if a number is non-zero:

```python
# Integer
int_number = 42
if bool(int_number):
    print("The integer is non-zero.")
else:
    print("The integer is zero.")
    
# Float
float_number = 3.14
if bool(float_number):
    print("The float is non-zero.")
else:
    print("The float is zero.")
```

#### Using integer values as boolean flags:

```python
flag = 1  # 1 represents True, 0 represents False
if bool(flag):
    print("The flag is set.")
else:
    print("The flag is not set.")

```

#### Checking if a string is empty:

```python
text = "Hello, World!"
if bool(text):
    print("The string is not empty.") # This gets displayed
else:
    print("The string is empty.")

text2 = ""
if bool(text2):
    print("The string is not empty.")
else:
    print("The string is empty.") # This gets displayed
```

#### Validating user input:

```python
user_input = input("Enter your name: ")
if bool(user_input):
    print(f"Hello, {user_input}!")
else:
    print("You did not enter a name.")
```

## F-Strings

F-strings are a way of **formatting** strings in Python 3.6 and later versions. They allow for the embedding of **expressions** inside string literals, using curly braces `{}` to enclose them.

Here's an example of an f-string:

```python
name = 'Alice'
age = 25
print(f'My name is {name} and I am {age} years old.')
```

Output:

```
My name is Alice and I am 25 years old.
```

In this example, the variables name and age are **embedded** into the string using curly braces. The **f** before the string indicates that it's an f-string.

You can also perform **operations** inside the curly braces. For example:

```python
x = 10
print(f'The square of {x} is {x**2}.')
```

Output:

```
The square of 10 is 100.
```


In addition, you can use **format specifiers** inside the curly braces to **control** the format of the output. For example:

```python
num = 3.141592653589793
print(f'The value of pi is approximately {num:.2f}.')
```

Output:

```
The value of pi is approximately 3.14.
```

In this example, the format specifier `:.2f` is used to specify that the value of `num` should be formatted as a **floating-point** number with **two** decimal places.

## Comments

In Python, **comments** are used to provide information or explanations about the code for future reference or to help other programmers understand your code. Python provides two ways to write comments: **single-line** comments and **multi-line** comments.

**Single-line comments** start with a hash symbol (`#`) and continue until the end of the line. Here's an example of a single-line comment:

```python
# This is a single-line comment
print("Hello, World!")
```
In this example, the comment explains that it's a single-line comment and **doesn't** affect the execution of the code.

**Multi-line comments**, also known as **block** comments, are enclosed in **triple** quotes (""" """) or (''' ''') and can span **multiple** lines. Here's an example of a multi-line comment:

```python
"""
This is a multi-line comment
It can span multiple lines
and is enclosed in triple quotes
"""
print("Hello, World!")
```

In this example, the **multi-line comment** explains how to write a multi-line comment and **doesn't** affect the execution of the code.

It's **essential** to write comments to make your code more **understandable**, especially when working on large and complex projects. Comments also help **other** programmers who work with your code to **understand** it better.

# Byte to Go

## Simple Calculator

Create a simple calculator that takes two numbers and an arithmetic operator as input from the user, performs the calculation, and displays the result. Incorporate all concepts learned in this lesson.

Here is some code to get you started. Use the last 3 comments on lines `11`, `14` and `17` as a guide to complete the task.

```python
# Get the first number from the user and convert it to a float
num1 = float(input("Enter the first number: "))

# Get the second number from the user and convert it to a float
num2 = float(input("Enter the second number: "))

# Get the arithmetic operator from the user
operator = input("Enter an arithmetic operator (+, -, *, /): ")


# Initialize the result variable


# Perform the calculation based on the input operator


# Display the result if the calculation was performed


```

## Amusement Park Ride Eligibility Checker

An amusement park has 6 rides with different age, height, and parental supervision requirements:

| Ride           | Minimum Age | Minimum Height | Maximum Height | Parental Requirement                                    |
| -------------- | ----------- | -------------- | -------------- | ------------------------------------------------------- |
| Merry-Go-Round | 2 years     | 3 feet         | 5 feet         | Required if under 4 years old                           |
| Kiddie Coaster | 4 years     | 3.5 feet       | 4.5 feet       | Required if under 6 years old or height below 3.67 feet |
| Bumper Cars    | 6 years     | 3.5 feet       | N/A            | Required if under 8 years old                           |
| Giant Swing    | 8 years     | 4 feet         | N/A            | N/A                                                     |
| Roller Coaster | 10 years    | 4.5 feet       | N/A            | N/A                                                     |
| Ferris Wheel   | N/A         | N/A            | N/A            | Required if under 5 years old or height below 3.5 feet  |

Write a program that asks the user for the child's name, age, and height, and then displays a message telling the parent which rides the child can go on, and if applicable, which rides they would need parent supervision for.

Here is some code to get you started. 

```python
# Get the child's name, age, and height from the user
name = input("Enter the child's name: ")
age = int(input("Enter the child's age (in years): "))
height = float(input("Enter the child's height (in feet): "))

# Initialize variables to store the names of the rides the child can go on
# and the rides that require parental supervision
eligible_rides = ""
supervised_rides = ""

# Check each ride's requirements and update the ride variables accordingly
if age >= 2 and 3 <= height <= 5:
    eligible_rides += "Merry-Go-Round"
    if age < 4:
        supervised_rides += "Merry-Go-Round"
        
# Continue for other rides...

# Display the message with eligible rides and rides requiring parental supervision
if eligible_rides:
    print(f"{name} can go on the following rides: {eligible_rides}.")
    if supervised_rides:
      print(f"For the following rides, {name} will need parental supervision: {supervised_rides}.")
else:
    print(f"Sorry, {name} does not meet the requirements for any rides at this time.")


```

Here are 2 examples of how the output should look like:
```
Enter the child's name: Jack
Enter the child's age (in years): 12
Enter the child's height (in feet): 5
Jack can go on the following rides: Merry-Go-Round, Bumper Cars, Giant Swing, Roller Coaster.
```

```
Enter the child's name: Cathy
Enter the child's age (in years): 5
Enter the child's height (in feet): 3.5
Cathy can go on the following rides: Merry-Go-Round, Kiddie Coaster.
For the following rides, Cathy will need parental supervision: Kiddie Coaster.
```

# **Conclusion**

Congratulations on completing this lesson! You've learned about Python data types, built-in functions, type conversion, and how to apply these concepts in real-world projects like the simple calculator and the amusement park ride eligibility checker.

Understanding data types and built-in functions is **essential** to mastering Python. These concepts will form the **foundation** for more advanced programming topics and applications, such as **data manipulation, web development, and automation**.

As a quick recap, here's a cheat sheet of the code covered in this lesson:

1. Displaying text: `print("Hello, World!")`
2. Getting user input: `user_input = input("Enter your name: ")`
3. Arithmetic operations: `result = 5 + 3`, `result = 7 * 4`, etc.
4. Decision-making:
  ```python
  if age >= 18:
      print("You are an adult.")
  elif age >= 13:
      print("You are a teenager.")
  else:
      print("You are a child.")
  ```
5. Built-in functions: `len("Hello")`, `int("42")`, `str(42)`, etc.
6. Type conversion: `float(3)`, `bool(1)`, `int("5")`, etc.

Keep practicing and applying these concepts, and you'll be well on your way to becoming a proficient Python programmer. Good luck on your Python journey!



