# Introduction

Loops are an important part of programming because they let us run a block of code over and over again. Without loops, we'd have to manually run the same code over and over again to get the same result. For example, in a system for authenticating users, we might have to check the user's credentials more than once before we are sure they are who they say they are. Without loops, we would have to write the same code more than once, which is slow and can lead to mistakes.

Here's an example of what the code for user authentication might look like without using loops:

```python
username = "johndoe"
password = "password123"

authenticated = False

input_username = input("Enter your username: ")
input_password = input("Enter your password: ")
if input_username == username and input_password == password:
    authenticated = True
else:
    print("Access denied. Please try again.")

if not authenticated:
    input_username = input("Enter your username: ")
    input_password = input("Enter your password: ")
    if input_username == username and input_password == password:
        authenticated = True
    else:
        print("Access denied. Please try again.")

if not authenticated:
    input_username = input("Enter your username: ")
    input_password = input("Enter your password: ")
    if input_username == username and input_password == password:
        authenticated = True
    else:
        print("Access denied. Please try again.")
        
# continue repeating the same code until the user is authenticated
```
``
As you can see, as we add more checks for user authentication, the code gets more complicated and repeats itself. This is where loops are very helpful because they let us automate the repetitive task of checking user credentials and make it less likely that there will be mistakes in the code.

# What are loops?

In computer programming, loops are structures that let a set of instructions be repeated over and over again until a certain condition is met. Loops are an important part of automating tasks that are done over and over again, and they can help you write code that works better and faster.

# The while loop

The while loop is a type of loop that continues to execute a block of code as long as the specified condition is true. Here is the general syntax for a while loop:

```python
while condition:
    # code to execute while the condition is true
```

In the while loop, the condition is a boolean expression that is checked at the beginning of each iteration. If the condition is true, the code inside the loop is executed. If the condition is false, the loop exits and the program continues to the next statement.

# Examples

## Prints Numbers from 1-10

### Problem
Write a program that uses the `while` loop to print out numbers from 1-10. The output should look like this:
```
1
2
3
4
5
6
7
8
9
0
```

### Solution

```python
count = 1
while count <= 10:
    print(count)
    count += 1
```

In this example, the `count` variable is initialized to 1, and the while loop continues to execute as long as `count` is less than or equal to 10. Inside the loop, the current value of count is printed, and then count is incremented by 1. This process repeats until `count` is greater than 10, at which point the loop exits.

> [!info] Compound Assignment Operators
> In Python, the `+=` operator is a shorthand way of writing `x = x + y`. It's used to add the value of `y` to the existing value of `x`, and then assign the result back to `x`. This operator is often used in loops and other situations where you need to update a variable's value repeatedly.
> 
> There are several other similar operators in Python, including:
> 
> `-=`: This operator subtracts the value on the right-hand side from the value on the left-hand side, and assigns the result back to the left-hand side variable. For example, x -= y is the same as writing x = x - y.
> `*=`: This operator multiplies the value on the right-hand side by the value on the left-hand side, and assigns the result back to the left-hand side variable. For example, x *= y is the same as writing x = x * y.
> `/=`: This operator divides the value on the left-hand side by the value on the right-hand side, and assigns the result back to the left-hand side variable. For example, x /= y is the same as writing x = x / y.
> 
> These operators can save you time and make your code more concise, especially when you need to update variables in loops or other repetitive tasks.

### Challenges
1. Write a program to print the numbers descending from 10 to 1. The output should look like this:
```
10
9
8
7
6
5
4
3
2
1
```
2. Write a program to print the square of the numbers from 1 to 10. The output should look like this:
```
1
4
9
16
25
36
49
64
81
100
```
3. Write a program that asks the user for a number between 2 and 100. The program should then print the numbers from 1 to that number. The output should look like this:
```
Enter a number between 2 and 100: 5
1
2
3
4
5
```

## User Authentication

Let's see how loops can help us solve the user authentication problem we were presented with at the beginning of the lesson.

```python
username = "johndoe"
password = "password123"
authenticated = False

while not authenticated:
    input_username = input("Enter your username: ")
    input_password = input("Enter your password: ")
    
    if input_username == username and input_password == password:
        print("Access granted!")
        authenticated = True
    else:
        print("Access denied. Please try again.")
```

- We start by defining the correct username and password. 
- We then use a while loop with a condition that checks whether the user has been authenticated or not. 
- The authenticated variable is initially set to False. 
- Inside the loop, we prompt the user to enter their username and password. 
- We then check whether the input username and password match the correct credentials. 
	- If they do, we print a success message and set the authenticated variable to True, which will cause the loop to exit in the next iteration. 
	- If they do not, we print an error message and repeat the loop.

### Challenges
1. Instead of using the variable `authenticated` to track whether the user is authenticated or not, use a variable called `is`

## Print Event Numbers from 5 to 30

Write a program that uses the `while` loop to print all the even numbers between 5 and 30 (inclusive). The output should look like this:

```
6
8
10
12
14
16
18
20
22
24
26
28
30
```

```python
start_num = 5
end_num = 30
num = start_num

while num <= end_num:
    if num % 2 == 0:
        print(num)
    num += 1
```

In this solution, we first initialize start_num to 5, end_num to 30, and num to start_num. We then use a while loop to repeatedly check if num is less than or equal to end_num. Inside the loop, we use an if statement to check if num is even, and if it is, we print it to the console. Finally, we increment num by 1 in each iteration of the loop.

The reason we need to increment num in each iteration is to ensure that the loop eventually terminates. Without this step, the loop would continue running indefinitely, which is known as an infinite loop. By incrementing num, we ensure that it eventually becomes greater than end_num, which causes the loop to exit.

Using a while loop in this case is just an alternative to using a for loop. The while loop allows us to control the iteration manually, which can be useful in situations where we need to perform more complex conditional checks before each iteration.


# Exercises
1. Print all even numbers between two given numbers.
2. Print the reverse of a given number.
3. Generate a Fibonacci sequence up to a given number.
4. Count the number of digits in a given number.
5. Find the largest and smallest digit in a given number.


# Summary

In this lesson, you have learned about loops in programming, the while loop, and an example of how to use a while loop in Python. You have also seen a use case where loops are essential for automating repetitive tasks. With this knowledge, you can begin to write more efficient and effective code.