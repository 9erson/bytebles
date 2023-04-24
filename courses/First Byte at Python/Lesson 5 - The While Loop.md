
# Concepts
## While Loop
If you recall in previous lessons, we use the `if` statement to run a block of code if a condition is `True`. This condition must be a **boolean expression**. A boolean expression is a Python expression that evaluates to a bool. That is, `True` or `False`.

Consider the following code:

```python
name = input("Name? ")
age = input("Age? ")

print(f"{name} is {age} years old!")

if age >= 18:
	print(f"{name} is an adult.")
	print(f"{name} is eligible to vote.")
else:
	print(f"{name} is not an adult.")
	print(f"{name} is not eligible to vote.")
```

In the first example of running the code, let's enter the values `Sarah` and `20`. Here is how the code would run:
```
Name? Sarah
Age? 20
Sarah is an adult.
Sarah is eligible to vote.
```

In this next example of running the code, let's enter the values `Sarah` and `12`. Here is how the code would look now:
```
Name? Sarah
Age? 20
Sarah is not an adult.
Sarah is not eligible to vote.
```

Everything that is indented after the `if` statement is called a code block and executes if the `if` condition is met; i.e. the `if` statement condition evaluates to `True`. Everything after the `else` statement executes if the `if` condition is not met; i.e. The `if` statement condition evaluates to `False`.

The structure of a `while` loop is similar:
```python
SECRET = 'Fr0gger'

attempt = input("Can you guess the secret word? ")

while attempt != SECRET:
	print("Sorry! It's not that...")
	attempt = input("Can you guess the secret word? ")

print("You guessed it!")
```

Here are the similarities with the `if` statement:
1. They both rely on criteria that is expressed as a boolean expression.
2. They both end with a `:` (colon).
3. They both are followed by one or more indented lines.

The difference with the `if` statement, however, is that the code block belonging to the `while` statement continues to run until the condition is `True`

A very common mistake beginners make is that the variable(s) within the criteria is never updated, and so the loop never ends. This is called an infinite loop. Although there are cases where an infinitive loop is required, in most cases, it's not.
Here is an example of the previous code, where the programmer forgot to update a variable included in the while criteria.

```python
SECRET = 'Fr0gger'

attempt = input("Can you guess the secret word? ")

while attempt != SECRET:
	print("Sorry! It's not that...")

print("You guessed it!")
```

Since the value of `attempt` never changes, unless the user successfully enters the secret on the first attempt, the code block will keep getting executed.

## Chew the byte
1. Ask the user to create a new password. Ensure the password is at least 10 characters long. Hint - use the `len` function.
	1. If the user enters a password that is less than 10 characters long, print the message `"The password should be at least 10 characters long. Try again."` Keep prompting the user until the user enters a password that is at least 10 characters long.
	2. After the user enters a password that is at least 10 characters long, print the message, "You have created a valid password."

## Looping n Times
In the case of the `while` loop examples so far, the number of times the loop takes place is not known beforehand. It would depend on the user. It could loop 0 times, or 1000 times, or even more! There are times when we may know, beforehand, how many times to run a piece of code.
Let's say you want to print out the numbers from 1 to 10, one on each line. Here is how you would do it.

```python
count = 1

while count <= 10:
	print(count)
	count += 1
```

### Chew the byte
1. Write a python program to print "Hello" (or some other string) 10 times.
2. Write a python program to print all the even numbers from 1 to 100.

## Break

There may be times when you may have to pre-maturely exit the loop. 
Suppose you want to write a program that asks the user to enter a password, but gives them only three chances to get it right. You can use a `while` loop to keep asking for input until the user enters the correct password or exhausts all three attempts, and use the `break` statement to exit the loop if the user enters the correct password:

```python
password = "secret"
attempts = 0

while attempts < 3:
    guess = input("Enter the password: ")
    if guess == password:
        print("You guessed the password! Access granted.")
        break
    else:
        print("Wrong password. Try again.")
        attempts += 1

if attempts == 3:
    print("Out of attempts. Access denied.")
```

### Chew the Byte
1. Write a program that asks the user to enter a series of positive numbers until they enter a negative number. You can use a `while` loop to keep asking for input until the user enters a negative number, and use the `break` statement to exit the loop. The first 2 lines have been done for you.
```python
while True:
    num = int(input("Enter a positive number (or a negative number to exit): "))

	# Your code here
```
2. Write a program that asks the user to enter a series of words, and stops asking when the user enters the word "quit". You can use a `while` loop to keep asking for input until the user enters the word "quit", and use the `break` statement to exit the loop. The first 2 lines have been done for you:

```python
while True:
    word = input("Enter a word (or 'quit' to exit): ")

	# Your code here
```

## Generating Random Numbers


# Byte to Go

## Number Guessing Game

Create a number guessing game where the user has to guess a secret number within a certain range. The program should provide feedback to the user after each guess, letting them know if their guess was too high or too low. The game should continue until the user guesses the correct number or decides to quit. 
Here is an example of what running the game should look like:
```
Guess the secret number (between 1 and 20): 3
Too low! Try again.
Guess the secret number (between 1 and 20): 16
Too high! Try again.
Guess the secret number (between 1 and 20): 10
Congratulations! You guessed the secret number!
```

If you're up for a challenge, here are three ideas to make the game more fun and interesting:

- Allow the user to choose the range of numbers they want to guess from
-   Limit the number of guesses the user can make before they lose the game
-   Keep track of the user's score based on the number of guesses it takes them to guess the correct number