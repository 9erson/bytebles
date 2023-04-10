
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

You have been asked to write a program for "Slice of Heaven Pizza," a local pizzeria, to help customers calculate their order total, including discounts, GST, and tip. In this fun and engaging exercise, you'll create a Pizza calculator that incorporates conditional statements using >, <, and, or, and not operators. Here are the detailed instructions for the enhanced Pizza calculator:

1. Begin by greeting the customer with a welcome message, such as "Welcome to Slice of Heaven Pizza Calculator!".
2. Prompt the customer to choose a pizza type (e.g., Pepperoni, Hawaiian, Vegetarian) and a pizza size (e.g., Small, Medium, Large).
3. Ask the customer if they would like to order wings. If yes, prompt them to enter the number of wings (e.g., 6, 8, or 12).
4. Ask the customer if they would like to order pop. If yes, prompt them to choose a pop size (e.g., Can, 500ml, or 2L) and a pop type (e.g., Coke, Sprite, etc.).
5. Request the customer to enter a coupon code if they have one (leave blank if not).
6. Calculate the prices for the chosen pizza, wings, and pop based on the customer's inputs. Use constants for the prices of each item and option.
7. Calculate the order subtotal by adding the prices of pizza, wings, and pop.
8. If the order subtotal is greater than $30, apply a 10% discount on the subtotal.
9. Check if the customer has ordered a large Pepperoni pizza and a 2L pop. If they have, congratulate them on unlocking a special offer and apply an additional $2 discount.
10. Apply a discount based on the customer's entered coupon code: $5 off for "SAVE5" or $10 off for "SAVE10".
11. Calculate the suggested tip amounts for 10%, 15%, and 20% of the subtotal, and display the suggested tips to the customer.
12. Prompt the customer to choose from the suggested tip amounts (10%, 15%, 20%) or input their own custom tip amount.
13. Calculate the GST as 5% of the subtotal.
14. Calculate the total amount by adding the subtotal, GST, and tip, and applying the discounts.
15. If the customer has not ordered any add-ons (wings or pop), display a friendly message to remind them to try these delicious options next time.
16. Display the order summary to the customer, including the pizza type and size, wings, pop type and size, subtotal, GST, discount, tip amount, and total.
17. By following these detailed instructions, you'll create a fun, interactive, and user-friendly Pizza calculator for "Slice of Heaven Pizza" that practices using different operators in conditional statements. Enjoy coding, and remember to treat yourself to a delicious slice of pizza afterwards!

To give you a head start, here is the first part of the program:

```python
# Pizza prices
PEPPERONI_PIZZA_PRICE_SMALL = 8.50
PEPPERONI_PIZZA_PRICE_MEDIUM = 12.50
PEPPERONI_PIZZA_PRICE_LARGE = 16.50

HAWAIIAN_PIZZA_PRICE_SMALL = 9.00
HAWAIIAN_PIZZA_PRICE_MEDIUM = 13.50
HAWAIIAN_PIZZA_PRICE_LARGE = 17.50

VEGETARIAN_PIZZA_PRICE_SMALL = 7.50
VEGETARIAN_PIZZA_PRICE_MEDIUM = 11.50
VEGETARIAN_PIZZA_PRICE_LARGE = 15.50

# Wings prices
WINGS_PRICE_6 = 5.00
WINGS_PRICE_8 = 6.50
WINGS_PRICE_12 = 9.00

# Pop prices
POP_PRICE_CAN = 1.00
POP_PRICE_500ML = 1.50
POP_PRICE_2L = 3.00

# Discount thresholds
DISCOUNT_THRESHOLD = 30
DISCOUNT_PERCENTAGE = 0.10

# Special offer for large Vegetarian pizza and 2L pop
SPECIAL_OFFER_DISCOUNT = 2

# Coupon codes and discounts
COUPON_SAVE5 = 5
COUPON_SAVE10 = 10

# GST rate
GST_RATE = 0.05

```

> [!Constants]
> In programming, a constant is a value that does not change throughout the execution of a program. It is a fixed value that remains the same throughout the life cycle of the program. Constants are used to represent values that should not be modified or reassigned during the program execution, providing a way to improve the readability and maintainability of the code.
> 
> The convention of using uppercase characters for constants is a widely followed practice in many programming languages, including Python. This convention makes it easier for developers to identify and distinguish constants from variables, which usually use lowercase characters. By using all uppercase characters, developers can quickly recognize that the value should not be changed, ensuring that the code is more understandable and less prone to errors.
> 
> In the provided code, we have defined several constants for prices, such as `PEPPERONI_PIZZA_PRICE_MEDIUM`, `HAWAIIAN_PIZZA_PRICE_SMALL`, `VEGETARIAN_PIZZA_PRICE_LARGE`, and various other prices for different items and options. These constants represent the fixed prices for each item or option, which should not change during the execution of the program. The use of constants in this context ensures that any changes to the prices can be made in a single location, making the code more maintainable and less prone to errors. It also improves the readability of the code, as it is clear that these values should not be modified during the program execution.
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

