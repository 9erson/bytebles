# Introduction



# Concepts

## Data Types

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

Functions are predefined pieces of code that perform a specific task. Python has many built-in functions. We have already been using some such as `print`, `input`, and `type`. Let's learn some more.

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