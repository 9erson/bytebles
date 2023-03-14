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

# Example of a while loop

Here is an example of a while loop that counts from 1 to 10:

```python
count = 1
while count <= 10:
    print(count)
    count += 1
```

In this example, the `count` variable is initialized to 1, and the while loop continues to execute as long as `count` is less than or equal to 10. Inside the loop, the current value of count is printed, and then count is incremented by 1. This process repeats until `count` is greater than 10, at which point the loop exits.

# User Authentication

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

# Exercises

Solve the following problems using the `while` loop:

1. Print all even numbers between two given numbers.
2. Print the reverse of a given number.
3. Generate a Fibonacci sequence up to a given number.
4. Count the number of digits in a given number.
5. Find the largest and smallest digit in a given number.


# Conclusion

In this lesson, you have learned about loops in programming, the while loop, and an example of how to use a while loop in Python. You have also seen a use case where loops are essential for automating repetitive tasks. With this knowledge, you can begin to write more efficient and effective code.