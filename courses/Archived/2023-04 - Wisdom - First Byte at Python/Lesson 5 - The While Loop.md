Welcome to this lesson on Python programming! In previous lessons, we've covered the fundamentals of **bools** and **boolean expressions**, as well as **decisions** (`if`, `elif`, `else`) in Python. Now, it's time to move on to a new concept - **loops**!

In this lesson, we will specifically be focusing on the `while` loop. A loop allows us to execute a block of code **multiple** times, which can save us a lot of time and effort when writing programs. We will also learn about generating **random numbers** in Python, which can add an element of **unpredictability** to our programs and make them more dynamic.

By the end of this lesson, you will have the knowledge and tools to create a fun and interactive **Number Guessing game** that incorporates **loops** and **random** numbers. This will test your understanding of the concepts we've covered so far, and help you reinforce your learning.

So, get ready to dive into the world of loops and random numbers in Python! Don't forget to complete the homework assignment, which will give you the chance to apply everything you've learned in this lesson. Good luck!

# Concepts

## While Loop

In previous lessons, we learned about the `if` statement, which allows us to run a block of code if a condition is `True`. This condition must be a **boolean expression** - an expression that evaluates to either `True` or `False`.

Now, let's talk about the `while` loop. Like the `if` statement, it relies on a boolean expression to control the flow of the program. However, instead of executing the code block only once, the `while` loop executes the code repeatedly **until** the boolean expression evaluates to `False`.

Here is an example of a `while` loop:

```python
SECRET = 'Fr0gger'

attempt = input("Can you guess the secret word? ")

while attempt != SECRET:
    print("Sorry! It's not that...")
    attempt = input("Can you guess the secret word? ")

print("You guessed it!")
```

In this example, the loop will keep executing the code block as long as the `attempt` variable is not equal to the `SECRET` variable. Once the user enters the correct value of `SECRET`, the boolean expression evaluates to `False`, and the loop ends.

Just like the `if` statement, the `while` loop ends with a colon (`:`) and is followed by one or more indented lines. The code block is executed repeatedly until the boolean expression evaluates to `False`.

One common mistake beginners make when using a `while` loop is **forgetting** to update the variable(s) in the boolean expression. If the variable(s) never change, the boolean expression will **always** evaluate to the same value, and the loop will become an **infinite loop**. 

> [!Infinite Loop]
> An infinite loop is a loop that never ends, and it can cause your program to crash or freeze.

Here is an example of an infinite loop:

```python
SECRET = 'Fr0gger'

attempt = input("Can you guess the secret word? ")

while attempt != SECRET:
    print("Sorry! It's not that...")
```

In this example, the `attempt` variable is **never** updated, so the boolean expression will always evaluate to `True`, and the loop will keep executing forever. To avoid this, make sure to update the variable(s) in the boolean expression within the loop.

## Chew the byte
1. Ask the user to create a new password. Ensure the password is at least 10 characters long. Hint - use the `len` function.
	1. If the user enters a password that is less than 10 characters long, print the message `"The password should be at least 10 characters long. Try again."` Keep prompting the user until the user enters a password that is at least 10 characters long.
	2. After the user enters a password that is at least 10 characters long, print the message, "You have created a valid password."

## Looping a Fixed Number of Times

In the previous examples, we used the `while` loop to repeat a block of code until a certain condition is met. However, there are times when we know beforehand how many times we need to repeat the code. In this case, we can use a `while` loop to achieve the same result.

### Example - Printing Numbers from 1 to 10

Let's say we want to print out the numbers from 1 to 10, one on each line. We can use a `while` loop to achieve this.

```python
count = 1

while count <= 10:
    print(count)
    count += 1
```

In the above code, we initialize a variable `count` to 1. Then we use a `while` loop to repeat the code block until `count` is greater than 10. Within the loop, we print the value of `count` and increment it by 1 at the end of each iteration.

### Chew the byte

1.  Write a Python program to print "Hello" 10 times using a `while` loop.
2.  Write a Python program to print all the even numbers from 1 to 100 using a `while` loop.

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

Random numbers are numbers that are selected in a way that is **unpredictable** and unbiased. In **Python**, you can generate random numbers using the built-in `random` module.

You can generate random numbers by using the `random.randint()` function. This function returns a random integer between two specified values, inclusive of both endpoints. Here's an example:

```python
import random

# Generate a random integer between 1 and 10
random_number = random.randint(1, 10)
print(random_number)
```

This tool can be useful in various real-world applications, such as games, simulations, testing, research, and encryption. For example, it can be used in **games** to simulate rolling a dice or selecting a random item from a list. In **scientific research**, it can be used to assign participants to different treatment groups or to generate random samples from a population. In **encryption**, it can be used to generate random numbers for encryption keys and to introduce randomness into encryption algorithms.

### Chew the Byte
1. Generate a random integer between 1 and 100 and print it to the console.
2. Generate a random integer between 1 and 6 (inclusive) to simulate a dice roll. Every time you run the code, you could see any **one** of the following:
	1. You rolled a 1.
	2. You rolled a 2.
	3. You rolled a 3.
	4. You rolled a 4.
	5. You rolled a 5.
	6. You rolled a 6.
3. Generate a random integer between 0 and 1 to simulate a coin toss. Every time you run the code, you should either get `Heads` or `Tails`.


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