## Introduction

The first time you've probably heard of a leap year was when you learned that famous rhyme as a kid. There are many versions of it, here is my favourite...

> Thirty days has September,  
> April, June, and November,  
> All the rest have thirty-one,  
> Save February at twenty-eight,  
> But leap year, coming once in four,  
> February then has one day more.

According to this rhyme, a leap year is every four years. But is it? 

Hi everyone, my name is Gerson. In this video, we're going to answer these four questions:

1. What is a leap year?
2. How do you tell if a year is a leap year?
3. Who came up with this calculation?
4. How do I write a simple python program to tell if a year is a leap year or not?

## What is a leap year?
So, let's start with the first question: What is a leap year? Simply put, a leap year is a year that has an extra day added to February, making it 29 days instead of the usual 28. This extra day is added to keep our calendar in sync with the earth's rotation around the sun, which takes approximately 365.24 days.

## How do you tell if a year is a leap year?
Now, how do you tell if a year is a leap year? The rule is that a year is a leap year if it is divisible by 4, except for years that are divisible by 100 but not divisible by 400. For example, the year 2000 was a leap year because it is divisible by 4 and 400, but the year 1900 was not a leap year because it is divisible by 4 and 100 but not divisible by 400.

## Who came up with this calculation?
As for who came up with this calculation, it can be traced back to the ancient Romans who first introduced the concept of leap years. However, it wasn't until the 16th century that the Gregorian calendar, which is the calendar we use today, was adopted and the rules for leap years were established.
It was introduced in 1582 by Pope Gregory XIII as a reform of the Julian calendar, which had been in use since 45 BCE. The Julian calendar had a small error in its calculation of the length of the year, which caused it to drift out of sync with the seasons over time.

## How do I write a simple python program to tell if a year is a leap year or not?
Lastly, for those who are interested in writing a simple python program to determine if a year is a leap year or not, stay tuned for the next part of this video where we'll walk you through the steps.

Here are the steps to write a Python program to determine if a year is a leap year or not:

Step 1: Ask the user to input a year.  
Step 2: Check if the year is divisible by 4. If the year is not divisible by 4, it is not a leap year.  
Step 3: If the year is divisible by 4, check if it is divisible by 100. If it is not divisible by 100, it is a leap year.  
Step 4: If the year is divisible by 100, check if it is divisible by 400. If it is divisible by 400, it is a leap year. If it is not divisible by 400, it is not a leap year.  
Step 5: Print the result.

```python
# Ask the user to input a year
year = int(input("Enter a year: "))

# Check if the year is a leap year
if year % 4 == 0:
    if year % 100 == 0:
        if year % 400 == 0:
            print(year, "is a leap year")
        else:
            print(year, "is not a leap year")
    else:
        print(year, "is a leap year")
else:
    print(year, "is not a leap year")
```

There is a simpler way to check if a year is a leap year. Instead of using nested if statements, you can use a single line of code that uses the **ternary operator** to check if the year is a leap year or not.

> [!Ternary Operator]
> The ternary operator is a shorthand way of writing an if-else statement in a single line of code. Its syntax is as follows:
> 
> ```python
> value_if_true if condition else value_if_false
> ```
> 
> Here's how it works:
> 
> 1.  The condition is evaluated first.
> 2.  If the condition is true, the expression returns `value_if_true`.
> 3.  If the condition is false, the expression returns `value_if_false`.

Here's what the code would look like:

```python
# Ask the user to input a year
year = int(input("Enter a year: "))

# Check if the year is a leap year
leap = "is" if year % 4 == 0 and (year % 100 != 0 or year % 400 == 0) else "is not"

# Print the result
print(year, leap, "a leap year")
```