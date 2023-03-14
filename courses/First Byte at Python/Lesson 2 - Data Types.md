# Introduction

In programming, a data type is an attribute of data which tells the compiler or interpreter how the programmer intends to use the data. In Python, data types are used to define the type of value that a variable can hold. In this lesson, we will explore the different data types available in Python, including strings, integers, and floats. We will also learn about type casting, which is the process of converting a value of one data type to another.

# Common Data Types

## Strings

In Python, a string is a sequence of characters. Strings are used to represent text data, and can be created using either single or double quotes. Here is an example:

```python
my_string = 'Hello, World!'
```

Strings can be indexed and sliced like lists, and have several built-in methods for manipulating text. For example, we can use the upper() method to convert all characters in a string to uppercase:

```python
my_string = 'hello, world!'
print(my_string.upper()) # Output: 'HELLO, WORLD!'
```

## Integers

In Python, an integer is a whole number. Integers can be positive or negative, and can be used to represent quantities, counts, or indices. Here is an example:

```python
my_integer = 42
```

Integers can be used in mathematical operations, such as addition, subtraction, multiplication, and division.

## Floats

In Python, a float is a decimal number. Floats can be used to represent real numbers, and are often used in scientific or mathematical applications. Here is an example:

```python
my_float = 3.14
```

Floats can also be used in mathematical operations, and can be converted to integers using type casting.

# Type Casting

In Python, type casting is the process of converting a value of one data type to another. This can be useful when we need to perform operations on values of different types. Here are some examples:

## Convert a string to an integer

```python
my_string = '42'
my_integer = int(my_string)
```

## Convert a float to an integer

```python
my_float = 3.14
my_integer = int(my_float)
```

## Convert an integer to a float

```python
my_integer = 42
my_float = float(my_integer)
```

# Exercises

1. Write a Python program that prompts the user to enter a weight in kilograms, and converts it to pounds. The conversion factor is 2.205 pounds per kilogram.
2. Write a Python program that prompts the user to enter a temperature in Celsius, and converts it to Fahrenheit. The conversion formula is `F = C * 1.8 + 32`.

# Summary

In this lesson, we learned about the different data types available in Python, including strings, integers, and floats. We also learned about type casting, which is the process of converting a value of one data type to another.