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
1. To keep track of whether the user is authenticated or not, use the variable named `unauthorized` instead of `authenticated`. Print the message "Access granted!" only if `unauthorized` is `False` i.e. the user has entered the correct username and password.
2. Modify the previous code to follow the conditions below:
	1. If the username and/or password is incorrect, show the message "Unknown user {input_username}", substituting {input_username} with the actual username provided by the user.
	2. If the username is correct (i.e., "johndoe"), but the password is incorrect, show the message "Incorrect password for user {input_username}", substituting {input_username} with the actual username provided by the user (which, in this case, will always be "johndoe").
	3. If both the username and password are correct, display the original message, "Access granted!"

## Print Even Numbers from 5 to 30

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

In this solution, we first initialize `start_num` to 5, `end_num` to 30, and `num` to `start_num`. We then use a while loop to repeatedly check if `num` is less than or equal to `end_num`. Inside the loop, we use an if statement to check if `num` is even, and if it is, we print it to the console. Finally, we increment `num` by 1 in each iteration of the loop.

The reason we need to increment `num` in each iteration is to ensure that the loop eventually terminates. Without this step, the loop would continue running indefinitely, which is known as an infinite loop. By incrementing `num`, we ensure that it eventually becomes greater than `end_num`, which causes the loop to exit.

### Challenges

Each challenge builds upon the previous and should be done in order.

1. The user should be able to provide values for `start_num` and `end_num`.
2. If the value entered for `end_num` is greater than the value entered for `start_num`, display an error message, and loop until `end_num` is greater than `start_num`.
3. If the value entered for either `end_num` or `start_num` is not a valid integer, display an error message, and loop until both `start_num` and `end_num` are both integers.

## Reverse a String

### Problem
Write a program that uses the `while` loop to reverse the string - `Hello`. 

```python
string = "Hello"
reversed_string = ""
index = len(string) - 1

while index >= 0:
    reversed_string += string[index]
    index -= 1

print(reversed_string)

# Output:
# olleH
```


### Explanation:

- The program initializes a variable string with the value "Hello". 
- It then initializes an empty string `reversed_string`, and a variable index with the value of the length of the string minus `1`. 
- The while loop runs as long as `index` is greater than or equal to `0`. 
- Inside the loop, it appends the character at the current index in string to `reversed_string`, and decrements the `index`. 
- Finally, it prints the reversed string.

> [!info] The `len()` Function
> The len() function is a built-in function in Python that returns the length of an object. The object can be a string, list, tuple, dictionary, or any iterable sequence.
> 
> The syntax of len() function is:
> 
> ```python
len(obj)
> ```
> where `obj` is the object whose length we want to find.
> 
> For example, to find the length of a string "Hello", we can use the len() function as follows:
> 
>```python
> string = "Hello"
> length = len(string)
> print(length)
> # Output:
> # 5
> ```
> In this example, the `len()`` function returns the length of the string "Hello", which is `5`, and stores it in the variable length. We then print the value of length using the `print()` function.


> [!info] Zero Based Counting
> In Python, as well as in many other programming languages, counting starts from 0, which means that the first element in a sequence is given an index of 0, the second element has an index of 1, and so on. This is known as 0-based counting or zero-indexed numbering.
> 
> For example, consider the string "Hello". The character 'H' is at index 0, 'e' is at index 1, 'l' is at index 2, 'l' is at index 3, and 'o' is at index 4.
> 
> ```
>  +---+---+---+---+---+
>  | H | e | l | l | o |
>  +---+---+---+---+---+
>    0   1   2   3   4
>  ```
> On the other hand, humans tend to use 1-based counting, which means that the first element in a sequence is given an index of 1, the second element has an index of 2, and so on.
> 
> For example, if we were counting the letters in the word "Hello" using 1-based counting, we would say that 'H' is at position 1, 'e' is at position 2, 'l' is at position 3, 'l' is at position 4, and 'o' is at position 5.
> 
> This difference in counting can sometimes cause confusion when working with code that uses zero-indexed numbering. It's important to remember that in Python, the first element in a sequence has an index of 0, not 1.
> 
> In general, zero-based counting is more common in programming because it is simpler and more efficient to implement in many cases. It also has some mathematical advantages when working with indices and offsets.

### Challenges
1. The user should be able to enter any text. The program should then reverse the text provided by the user.
2. If the text provided by the user is a palindrome, display the message - `"{user_input} is a palindrome!"`.

> [!info] Palindrome
> A palindrome is a word, phrase, number, or other sequence of characters that reads the same forward and backward. Examples - racecar, level, deified.

## Print a Fibonacci sequence up to a given number
### Problem

Write a program that uses the `while` loop to print the Fibonacci sequence from 1 to 100.

> [!info] Fibonacci sequence
> The Fibonacci sequence is a series of numbers in which each number is the sum of the two preceding numbers. The sequence starts with 0, 1, and each subsequent number is the sum of the previous two numbers. Therefore, the first few numbers in the Fibonacci sequence are:
> 
> 0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89, ...

### Solution

```python
a = 0
b = 1
count = 0
while b < 100:
    print(b)
    next_term = a + b
    a = b
    b = next_term
    count += 1
```

### Explanation
-   Initialize variables `a` to 0 and `b` to 1, the first two terms in the sequence
-   Initialize a counter variable `count` to 0
-   Use a `while` loop to print the sequence up to the first term greater than or equal to 100
-   In each iteration of the loop:
    -   Check if `b` is less than 100
    -   If it is, print `b` and calculate the next term in the sequence (`a + b`) and store it in `next_term`
    -   Update `a` to be the last term (`b`) and `b` to be the next term (`next_term`)
    -   Increment the counter variable `count` by 1
-   When `b` becomes greater than or equal to 100, the loop terminates and the program ends

### Challenges
- The user should be able to input a number `n` and have the program print the first `n` terms of the Fibonacci sequence, instead of printing up to a fixed value of 100.
- The user should be able to choose whether to print the Fibonacci sequence in reverse or forward order.

## Find the largest and smallest digit in a given number

### Problem
Write a python program to use the `while` loop to find the largest and smallest digit in a given number.

### Output Examples

```
# Example 1
number = 234567
Largest digit: 7
Smallest digit: 2

# Example 2
number = 987654321
Largest digit: 9
Smallest digit: 1
```
Examples



python
Copy code
num = int(input("Enter a number: "))
largest = 0
smallest = 9

while num > 0:
    digit = num % 10
    if digit > largest:
        largest = digit
    if digit < smallest:
        smallest = digit
    num = num // 10

print("Largest digit:", largest)
print("Smallest digit:", smallest)
Explanation

The program works as follows:

First, we take the input number from the user.
We initialize two variables largest and smallest to 0 and 9 respectively. These variables will hold the largest and smallest digits in the number.
We enter into a while loop which will continue until num becomes 0.
In each iteration of the loop, we extract the last digit of num using the modulus operator (%) and store it in a variable called digit.
We then compare digit with largest and smallest and update their values accordingly.
We then divide num by 10 using integer division (//) to remove the last digit from num.
Once the while loop terminates, we print the values of largest and smallest.
Challenges

Story 1: Allow negative input
As a user, I want to be able to input negative numbers so that I can find the largest and smallest digit in negative numbers as well.

Story 2: Handle non-numeric input
As a user, I want the program to handle non-numeric input so that the program does not crash and provides meaningful feedback.



Story 4: Handle decimal inputs
As a user, I want the program to handle decimal inputs so that I can find the largest and smallest digit in decimal numbers as well.



# Summary

In this lesson, you have learned about loops in programming, the while loop, and an example of how to use a while loop in Python. You have also seen a use case where loops are essential for automating repetitive tasks. With this knowledge, you can begin to write more efficient and effective code.