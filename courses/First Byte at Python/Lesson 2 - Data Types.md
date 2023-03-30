# Introduction

A data type is an attribute of data that tells the ==compiler== or ==interpreter== how the programmer plans to use it. In Python, data types tell you what kind of value a variable can have. In this lesson, we'll look at the different types of data that Python offers, such as strings, integers, and floats. We will also learn about type casting, which is how to change a value from one type of data to another.

> [!info] Compiler
A compiler is a program that translates source code into an executable program. In Python, the compiler translates the source code into a lower-level representation called byte code, which can be executed by the Python virtual machine.

> [!info] Interpreter
An interpreter is a program that reads and executes code line-by-line, without first converting it into an executable form. In Python, the interpreter reads the code line-by-line and executes it immediately.

# Concepts

## Common Data Types

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

## Type Casting

Type casting is a process of converting a value from one data type to another in Python. It can be helpful when we need to perform operations on values of different types.

Here are some examples:

- Convert an integer or float to a string using the `str()` function:

```python
my_integer = 42
my_float = 3.14

my_integer_str = str(my_integer)
my_float_str = str(my_float)
```

- Convert a string to an integer using the `int()` function:

```python
my_string = '42'
my_integer = int(my_string)
```

- Convert a float to an integer using the `int()` function:

```python
my_float = 3.14
my_integer = int(my_float)
```

- Convert an integer to a float using the `float()` function:

```python
my_integer = 42
my_float = float(my_integer)
```

## Built-in Functions

### `len()` - Returns the length of a string
```python
# Star Wars Example
quote = "May the Force be with you"
print(len(quote)) # Output: 24

# Lord of the Rings Example
ring_inscription = "One ring to rule them all, one ring to find them, one ring to bring them all, and in the darkness bind them."
print(len(ring_inscription)) # Output: 111

```


# Exercises

1. Write a Python program that prompts the user to enter a weight in kilograms, and converts it to pounds. The conversion factor is 2.205 pounds per kilogram.
2. Write a Python program that prompts the user to enter a temperature in Celsius, and converts it to Fahrenheit. The conversion formula is `F = C * 1.8 + 32`.

# Summary

In this lesson, we learned about the different data types available in Python, including strings, integers, and floats. We also learned about type casting, which is the process of converting a value of one data type to another.