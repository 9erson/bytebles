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
-   **Functions from external libraries**: External libraries are collections of functions that are not built into Python, but can be imported and used in your code. Examples include `numpy`, `pandas`, and `matplotlib`.
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

## F-Strings

As a recap, Python provides the `+` operator for string concatenation, which allows you to combine strings and variables. For example:

```python
name = "Alice"
age = 25
print("My name is " + name + " and I'm " + str(age) + " years old.")
```

However, this approach can be cumbersome and error-prone, especially when you need to format longer strings with multiple variables.

Fortunately, Python 3.6 introduced a new and easier way to format strings: f-strings. F-strings allow you to embed ==expressions== inside string literals using curly braces `{}`. For example:

```python
name = "Alice"
age = 25
print(f"My name is {name} and I'm {age} years old.")
```

> [!Expressions]
> In Python, an expression is a piece of code that produces a value. An expression can be as simple as a single variable, or it can be a complex combination of variables, functions, and operators.
> 
> ```python
> # A simple expression that assigns the value 5 to the variable x
> x = 5
> 
> # A more complex expression that adds two numbers together
> y = 10 + 7
> 
> # An expression that multiplies two variables and stores the result in a new variable
> a = 3
> b = 4
> c = a * b
> 
> # An expression that concatenates two strings
> hello = "Hello"
> name = "Alice"
> greeting = hello + " " + name
> 
> # An expression that divides two numbers and returns a float
> m = 10
> n = 3
> result = m / n
> ```
> 

In this example, we use an f-string to format the string `"My name is {name} and I'm {age} years old."`. The expressions inside the curly braces are evaluated and replaced with their values, resulting in the same output as the previous example.

F-strings offer several advantages over string concatenation using the `+` operator. First, they are more concise and readable. Second, they automatically handle type conversion, so you don't need to manually convert variables to strings using the `str()` function. Third, they are more efficient because they only evaluate the expressions inside the curly braces once, whereas string concatenation may need to create multiple intermediate strings.

Overall, f-strings are a convenient and efficient way to format strings in Python, and are recommended over string concatenation using the `+` operator.

# Byte to Go

### Pizza Calculator

You're working as a software engineer in a pizzeria, and your boss has asked you to build a program to calculate the price of a customer's order. Use the following ==constants==:

```python
PIZZA_PRICE = 10.99    # Price of one pizza
TOPPING_PRICE = 1.50   # Price of one topping
WINGS_PRICE = 7.99     # Price of one serving of wings
POP_PRICE = 1.50       # Price of one can of pop
GST_RATE = 0.05        # GST rate
TIP_RATE = 0.15        # Suggested tip rate
```

> [!Constants]
> In programming, constants are values that do not change during the execution of the program. They are often given a name in upper case letters to differentiate them from variables that can change.
> 
> In Python, there is no way to force a variable to be constant, but it is common practice to name constants in upper case letters to indicate that they should not be changed. However, this convention is not enforced by the Python language itself, and it is still possible to change the value of a constant if a programmer chooses to do so.
> 
> Constants are often used to store values that are used repeatedly in a program, such as fixed prices, tax rates, or other important values. By using constants, the program can easily adjust the values of these parameters in one place, rather than changing them repeatedly throughout the program.
> 
> For example, in the pizza calculator program, the `PIZZA_PRICE`, `TOPPING_PRICE`, `WINGS_PRICE`, `POP_PRICE`, `GST_RATE`, and `TIP_RATE` are all constants that have fixed values that are used in the calculations. These constants are named in upper case letters to indicate that they should not be changed, even though Python does not enforce this convention.

Write a Python program that:

1.  Greets the customer with the message "Welcome to Slice of Heaven Pizza Calculator!"
2.  Asks the customer for the number of servings of three different toppings (pepperoni, mushrooms, onions), the number of servings of wings, and the number of cans of pop they would like to order, using the `input()` function.
3.  Calculates the suggested tip, which is equal to 15% of the subtotal (pizza price + wings price + pop price), rounded to 2 decimal places, using the `round()` function.
4.  Asks the customer how much they would like to tip, with the suggested tip amount as a default value, using the `input()` function.
5.  Calculates the subtotal, GST (5% of the subtotal), and total (subtotal + GST + tip), rounding the total to 2 decimal places using the `round()` function.
6.  Displays the order summary to the customer, including the pizza price, topping price, wings price, pop price, subtotal, GST, suggested tip, tip amount, and total, each rounded to 2 decimal places.

This is what running the program may look like:

```
Welcome to Slice of Heaven Pizza Calculator!

Please select your toppings:
How many servings of pepperoni do you want?  1
How many servings of mushrooms do you want?  0
How many servings of onions do you want?  1
How many servings of wings do you want? 1
How many cans of pop do you want? 1
How much would you like to tip (15% suggested)? $ 4
Your order summary for Slice of Heaven Pizza:

- Pizza price: $10.99
- Topping price: $3.0
- Wings price: $7.99
- Pop price: $1.5
- Subtotal: $23.48
- GST (5%): $1.1740000000000002
- Suggested tip (15%): $3.07
- Tip: $4.0
- Total: $28.65
```
