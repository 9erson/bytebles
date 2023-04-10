
# Concepts
## Boolean Data Type

In Python, the boolean data type is represented by the bool class, and it has two possible values: True and False. Booleans can be assigned to variables, just like any other data type:

```python
x = True
y = False
```

Booleans can also be created by using comparison operators and logical operators, which we will cover in the next sections.


## Comparison Operators

Comparison operators are used to compare two values and return a boolean value indicating whether the comparison is true or false. Here are the comparison operators in Python:

| Operator | Description              |
|:--------:| ------------------------ |
|    ==    | Equal                    |
|    !=    | Not Equal                |
|    >     | Greater than             |
|    <     | Less than                |
|    <=    | Greater than or equal to |
|    <=    | Less than or equal to                         |

Here's an example of using comparison operators:

```python
x = 10
y = 5

print(x > y)   # Output: True
print(x == y)  # Output: False
print(x != y)  # Output: True
```

  > [!hint] Hint
  > ### The Modulo Operator
To check whether a number is even or odd, you can use the modulo operator %. The modulo operator returns the remainder of a division operation. If a number is even, it will have no remainder when divided by 2. If a number is odd, it will have a remainder of 1 when divided by 2. Here are two examples of using the modulo operator:
> ```python
10 % 2
5 % 2

### Chew the Byte
1. Write a boolean expression to determine if the variable `temp` is freezing. (0 degrees Celsius).
2. Write a boolean expression to determine if a number is odd.
3. Write a boolean expression to determine if the variable `age` is an adult.

## Logical Operators

Logical operators are used to combine boolean values and return a boolean value. Here are the logical operators in Python:

| Operator | Description                                  |
| -------- | -------------------------------------------- |
| and      | Returns True if both operands are True       |
| or       | Returns True if at least one operand is True |
| not      | Returns True if the operand is False                                             |

>[!info] Operand
>In computer programming, an operand is a value or expression on which a mathematical, logical or bitwise operation is performed. In other words, it's an input to an operator that is used to produce a result. For example, in the expression `5 + 7`, the operands are `5` and `7`, and the operator is `+`. Similarly, in the expression `x > 10`, the operand is `x`, and the operator is `>`. In general, operands can be constants, variables, or expressions that evaluate to a value.

Here's an example of using logical operators:

```python
x = 10
y = 5
z = 7

print(x > y and z > y)  # Output: True
print(x > y or z < y)   # Output: True
print(not x > y)        # Output: False
```

### Chew the Byte
1. Write a boolean expression to determine if the variable `year` is a leap year. 1.  A year is a leap year if it is divisible by 4, but not divisible by 100, unless it is divisible by 400.
2. Write a boolean expression to determine if a triangle is valid: Given three side lengths `a`, `b`, and `c`, determine if they form a valid triangle. A triangle is valid if the sum of the lengths of any two sides is greater than the length of the third side.

## Conditional Statements

Conditional statements are used to execute different blocks of code based on whether a condition is true or false. In Python, we use `if`, `elif`, and `else` statements to create conditional statements.

>[!info] Statement
>In Python, a statement is a line of code that performs a specific action. A statement can be a simple expression or a complex block of code, and it can perform various operations, such as assigning values to variables, executing loops, or making decisions based on conditions.


### If
Here's the syntax for an if statement:

```python
if condition:
    # code to execute if condition is true
```

### Else

Here's the syntax for an if statement with an else block:

```python
if condition:
    # code to execute if condition is true
else:
    # code to execute if condition is false
```

### Elif
And here's the syntax for an if statement with multiple elif blocks and an else block:

```python
if condition1:
    # code to execute if condition1 is true
elif condition2:
    # code to execute if condition2 is true
elif condition3:
    # code to execute if condition3 is true
else:
    # code to execute if all conditions are false
```

### Example 
Here's an example of using conditional statements:
```python
x = 10
y = 5

if x > y:
    print("x is greater than y")
elif x < y:
    print("y is greater than x")
else:
    print("x and y are equal")

# Output:
# x is greater than y
```


### Chew the Byte

1. Write a Python program that asks the user to enter a number, and checks whether the number is even or odd. If the number is even, the program should print "The number is even." If the number is odd, the program should print "The number is odd."
2. Write a Python program that asks the user for their age and prints out their corresponding life stage based on the following criteria:
	- If the age is between 0 and 2 (inclusive), print "Infant"
	- If the age is between 3 and 4 (inclusive), print "Toddler"
	- If the age is between 5 and 12 (inclusive), print "Child"
	- If the age is between 13 and 17 (inclusive), print "Teenager"
	- If the age is 18 or older, print "Adult"

> [!info] Inclusive
> Inclusive refers to the property of encompassing the endpoint values of a given range or category. For example, in the code provided, the age ranges are defined as inclusive, meaning that if an age falls on the upper or lower end of a given range, it will be classified as belonging to the corresponding life stage.

# Byte to Go

## Pizza Calculator - II

Write a python program, similar to the last one, that asks the user details for their order, then calculates their total. Here are the detailed requirements.

1.  Define ==constants== for pizza prices (Pepperoni, Hawaiian, Vegetarian), pizza sizes, wings, and pop sizes and types.
2.  Greet the customer with a welcome message.
3.  Ask the customer for their pizza choice (Pepperoni, Hawaiian, or Vegetarian) and store it in a variable.
4.  Ask the customer for their pizza size (small, medium, or large) and store it in a variable.
5.  Calculate the pizza price based on the customer's choices.
6.  Ask the customer if they would like wings, and if yes, ask for the number of wings (6, 8, or 12) and calculate the wings price.
7.  Ask the customer if they would like pop, and if yes, ask for the size (can, 500ml, or 2L) and type (Coke, Sprite, etc.) of pop, then calculate the pop price.
8.  Calculate the subtotal by adding the prices of pizza, wings, and pop.
9.  Calculate the suggested tip amounts for 10%, 15%, and 20%.
10. Prompt the customer to choose from the suggested tip amounts or input their own tip amount.
11.  Calculate the GST (5% of the subtotal).
12.  Calculate the total amount by adding the subtotal, GST, and tip.
13.  Display the order summary, including the pizza price, wings price, pop price, subtotal, GST, tip amount, and total.

To give you a head start, I've done step 1 for you:

```python
# Constants for prices 
PEPPERONI_PIZZA_PRICE = 10.00 
HAWAIIAN_PIZZA_PRICE = 12.00 
VEGETARIAN_PIZZA_PRICE = 9.00 
SMALL_SIZE_PRICE = 0 
MEDIUM_SIZE_PRICE = 2.00 
LARGE_SIZE_PRICE = 4.00 
WINGS_6_PRICE = 5.00 
WINGS_8_PRICE = 6.50 
WINGS_12_PRICE = 9.50 
CAN_PRICE = 1.25 
BOTTLE_500ML_PRICE = 2.00 
BOTTLE_2L_PRICE = 3.50
```

> [!Constants]
> In programming, a constant is a value that does not change throughout the execution of a program. It is a fixed value that remains the same throughout the life cycle of the program. Constants are used to represent values that should not be modified or reassigned during the program execution, providing a way to improve the readability and maintainability of the code.
> 
> The convention of using uppercase characters for constants is a widely followed practice in many programming languages, including Python. This convention makes it easier for developers to identify and distinguish constants from variables, which usually use lowercase characters. By using all uppercase characters, developers can quickly recognize that the value should not be changed, ensuring that the code is more understandable and less prone to errors.
> 
> In the provided code, we have defined several constants for prices, such as `PEPPERONI_PIZZA_PRICE`, `HAWAIIAN_PIZZA_PRICE`, `VEGETARIAN_PIZZA_PRICE`, and various other prices for different items and options. These constants represent the fixed prices for each item or option, which should not change during the execution of the program. The use of constants in this context ensures that any changes to the prices can be made in a single location, making the code more maintainable and less prone to errors. It also improves the readability of the code, as it is clear that these values should not be modified during the program execution.
> 
> In some programming languages, constants are defined using special keywords that enforce immutability, meaning their values cannot be changed once assigned. This helps prevent accidental modification of these values, which could lead to unexpected behavior or errors. Attempting to change the value of a constant in such languages would result in a compilation failure, alerting the developer of the issue before the program is executed.
> 
> For example, languages like C, C++, and Java use the `const` or `final` keyword to define constants:
> 
> C and C++:
> 
> ```c
> const int SPEED_OF_LIGHT = 299792458;
> ```
> 
> Java:
> ```java
> public static final int SPEED_OF_LIGHT = 299792458;
> ```
> 
> Python, however, does not have a built-in way to enforce immutability of variables. There is no specific keyword or feature to prevent the modification of a constant value. Instead, the convention of using uppercase characters for constant names is followed to signal to other developers that the value should not be modified. This convention relies on the programmer's discipline not to change the value, as the language itself does not enforce immutability.

