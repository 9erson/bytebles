# Introduction

Booleans are a fundamental data type in Python that represent true or false values. They are often used in control flow statements, such as conditional statements, to make decisions based on whether a condition is true or false. In this lesson, we will cover the boolean data type, comparison operators, logical operators, and conditional statements in Python.

# Boolean Data Type

In Python, the boolean data type is represented by the bool class, and it has two possible values: True and False. Booleans can be assigned to variables, just like any other data type:

```python
x = True
y = False
```

Booleans can also be created by using comparison operators and logical operators, which we will cover in the next sections.

## Boolean Related Operators

### Comparison Operators

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

### Logical Operators

Logical operators are used to combine boolean values and return a boolean value. Here are the logical operators in Python:

| Operator | Description                                  |
| -------- | -------------------------------------------- |
| and      | Returns True if both operands are True       |
| or       | Returns True if at least one operand is True |
| not      | Returns True if the operand is False                                             |

```ad-info
**Operand:**

In computer programming, an operand is a value or expression on which a mathematical, logical or bitwise operation is performed. In other words, it's an input to an operator that is used to produce a result. For example, in the expression `5 + 7`, the operands are `5` and `7`, and the operator is `+`. Similarly, in the expression `x > 10`, the operand is `x`, and the operator is `>`. In general, operands can be constants, variables, or expressions that evaluate to a value.
```

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

Conditional statements are used to execute different blocks of code based on whether a condition is true or false. In Python, we use if, elif, and else statements to create conditional statements.

```ad-info
**Statement:**

In Python, a statement is a line of code that performs a specific action. A statement can be a simple expression or a complex block of code, and it can perform various operations, such as assigning values to variables, executing loops, or making decisions based on conditions.
```

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

# Exercise

## Even or Odd

Write a Python program that asks the user to enter a number, and checks whether the number is even or odd. If the number is even, the program should print "The number is even." If the number is odd, the program should print "The number is odd."

### The Modulo Operator
To check whether a number is even or odd, you can use the modulo operator %. The modulo operator returns the remainder of a division operation. If a number is even, it will have no remainder when divided by 2. If a number is odd, it will have a remainder of 1 when divided by 2. Here's an example of using the modulo operator:

```python
number = 10

if number % 2 == 0:
    print("The number is even.")
else:
    print("The number is odd.")
```

## Age-Based Life Stage Classifier

Write a Python program that asks the user for their age and prints out their corresponding life stage based on the following criteria:

- If the age is between 0 and 2 (inclusive), print "Infant"
- If the age is between 3 and 4 (inclusive), print "Toddler"
- If the age is between 5 and 12 (inclusive), print "Child"
- If the age is between 13 and 17 (inclusive), print "Teenager"
- If the age is 18 or older, print "Adult"

```ad-info
In this context, "inclusive" means that the age values being checked in the code are considered part of the corresponding life stage. For example, if the age is 2, the code will print "Infant" because the age of 2 is included in the range of ages defined for the "Infant" life stage (0-2 years old). Similarly, if the age is 4, the code will print "Toddler" because the age of 4 is included in the range of ages defined for the "Toddler" life stage (3-4 years old). If the code were not inclusive, it would not consider the upper limit of the range as part of the corresponding life stage and would exclude some individuals who fall within that range.
```

# Summary

In this lesson, we covered the boolean data type, comparison operators, logical operators, and conditional statements in Python.