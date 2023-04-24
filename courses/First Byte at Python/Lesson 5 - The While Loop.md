
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
There may be times when you may have to pre-maturely exit the loop. Let's say you want to print the numbers from 1 to 10, but at the


```

# Byte to Go
Write a python program that prints