
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

### Chew the Byte


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


# Exercises

- Write a Python program that asks the user to enter a number, and checks whether the number is even or odd. If the number is even, the program should print "The number is even." If the number is odd, the program should print "The number is odd."
  > [!hint] Hint
  > ### The Modulo Operator
To check whether a number is even or odd, you can use the modulo operator %. The modulo operator returns the remainder of a division operation. If a number is even, it will have no remainder when divided by 2. If a number is odd, it will have a remainder of 1 when divided by 2. Here are two examples of using the modulo operator:
> ```python
10 % 2
5 % 2

- Write a Python program that asks the user for their age and prints out their corresponding life stage based on the following criteria:
	- If the age is between 0 and 2 (inclusive), print "Infant"
	- If the age is between 3 and 4 (inclusive), print "Toddler"
	- If the age is between 5 and 12 (inclusive), print "Child"
	- If the age is between 13 and 17 (inclusive), print "Teenager"
	- If the age is 18 or older, print "Adult"

> [!info] Inclusive
> Inclusive refers to the property of encompassing the endpoint values of a given range or category. For example, in the code provided, the age ranges are defined as inclusive, meaning that if an age falls on the upper or lower end of a given range, it will be classified as belonging to the corresponding life stage.


# Summary

In this lesson, we covered the boolean data type, comparison operators, logical operators, and conditional statements in Python.