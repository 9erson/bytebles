# Introduction

Welcome to this Python lesson focusing on data types, type casting, and functions! In this lesson, we will dive deeper into the core concepts that play a crucial role in Python programming. Whether you are working with text data, performing mathematical operations, or writing ==reusable code==, understanding these concepts is essential for efficient and effective Python development.

> [!Reusable Code]
> "Reusable code" is a programming concept where pieces of code are written in such a way that they can be used multiple times in different parts of a program, or even in other projects, without having to rewrite the same code. This approach saves time, reduces the chance of errors, and makes the code more maintainable and easier to understand. In simple terms, reusable code is like a recipe that can be followed multiple times to create the same dish, without needing to come up with a new recipe each time.

# Concepts

## Data Types

Python is a versatile and powerful programming language that offers a wide range of built-in data types to help you store and manipulate information. Understanding these data types is crucial for writing effective Python code, as they determine how values can be stored, processed, and interacted within your programs. In this section, we will discuss some of the most commonly used data types in Python, including strings, integers, and floats, and explore their properties and use cases through examples.

Now, let's dive into each of these data types in more detail:

### Strings

In Python, a string is a sequence of characters. Strings are used to represent text data, and can be created using either single or double quotes. Here is an example:

```python
my_string = 'Hello, World!'
```

### Integers

In Python, an integer is a whole number. Integers can be positive or negative, and can be used to represent quantities, counts, or indices. Here is an example:

```python
my_integer = 42
```

Integers can be used in mathematical operations, such as addition, subtraction, multiplication, and division.

### Floats

In Python, a float is a decimal number. Floats can be used to represent real numbers, and are often used in scientific or mathematical applications. Here is an example:

```python
my_float = 3.14
```

Floats can also be used in mathematical operations, and can be converted to integers using type casting.

### Chew the Byte
1. Which data type should you use to store your name?
2. Which data type should you use to store your age?
3. What is the data type of the result of adding 2 integers?
4. What is the data type of the result of adding 2 floats?
5. What is the data type of the result of adding an integer and a float?
6. What is the data type of the result of dividing one integer from another?

## Type Casting

Type casting is a process of converting a value from one data type to another in Python. It can be helpful when we need to perform operations on values of different types.

Here are some examples:

### Integer or Float to String

Convert an integer or float to a string using the `str()` function:

```python
my_integer = 42
my_float = 3.14

my_integer_str = str(my_integer)
my_float_str = str(my_float)
```

### String to Integer

Convert a string to an integer using the `int()` function:

```python
my_string = '42'
my_integer = int(my_string)
```

### Float to Int

Convert a float to an integer using the `int()` function:

```python
my_float = 3.14
my_integer = int(my_float)
```

### Integer to Float

Convert an integer to a float using the `float()` function:

```python
my_integer = 42
my_float = float(my_integer)
```

### Chew the Byte
1. Write a Python program that prompts the user to enter a weight in kilograms, and converts it to pounds. The conversion factor is 2.205 pounds per kilogram.
2. Write a Python program that prompts the user to enter a temperature in Celsius, and converts it to Fahrenheit. The conversion formula is `F = C * 1.8 + 32`.

## Functions

Functions are reusable pieces of code that perform a specific task. They help to organize, modularize, and simplify your code. Functions can be built-in or custom, and they can come from external libraries.

Here are some important concepts related to functions:

-   **Name of the function**: Functions have unique names that are used to call them. For example, `print` is the name of the function that outputs text to the console.
-   **Parentheses**: Functions are followed by parentheses, which may contain arguments or parameters.
-   **Arguments or parameters**: Functions can take input values, known as arguments or parameters, to perform a specific task. These values are passed to the function inside the parentheses.
-   **Built-in functions**: Python has a set of built-in functions, like `print`, `input`, and `type`, that come with the language and are always available for use.
-   **Custom functions**: You can define your own functions, known as custom functions, to perform specific tasks. We'll learn how to write custom functions in a later lesson.
-   **Functions from external libraries**: External libraries are collections of functions that are not built into Python but can be imported and used in your code. Examples include `numpy`, `pandas`, and `matplotlib`.
-   **Optional parameters**: Some functions have optional parameters with default values. If you don't provide a value for an optional parameter, the function will use the default value.
-   **Return value**: Functions can return a value, which is the result of their computation. The `return` keyword is used to specify the value to be returned.
-   **Return type**: The return type is the data type of the value returned by a function. It can be any data type, such as `int`, `float`, `str`, or even custom data types.
-   **Parameter types**: Functions can accept parameters of various types, like `int`, `float`, `str`, and more. The type of a parameter often determines how the function behaves.

We have already used some built-in functions like `print`, `input`, and `type`. Let's take a look at some more built-in functions.

### `len()` - Returns the length of a string

```python
quote = "May the Force be with you"
print(len(quote)) # Output: 24

ring_inscription = "One ring to rule them all, one ring to find them, one ring to bring them all, and in the darkness bind them."
print(len(ring_inscription)) # Output: 111

```

### `abs()` - Returns the absolute value of a number

```python
print(abs(-33))
print(abs(-0.66))
print(abs(35))
```

### `round()` - Rounds a number to the nearest integer or to the specified number of decimals

```python
print(round(3.14159))
print(round(3.14159, 2))
```

### Chew the Byte
1. Write a program that takes the temperature in Celsius for two different days and calculates the absolute difference in temperatures.
2. A hiker starts and ends their hike at different altitudes (measured in meters). Calculate the absolute difference in altitude between the starting and ending points.