# Introduction

Welcome to the Introduction to Python course, where we will discuss the IPO model and its application to programming. The IPO model is a fundamental concept in programming that describes the flow of data within a program. The model consists of three main components: Input, Processing, and Output. In this lesson, we will discuss these components and their implementation in Python.

>[!info] Program
> A set of instructions written in a programming language that a computer can interpret and execute to perform a specific task or solve a problem.


## IPO Model - Input, Processing, Output

The IPO model describes the flow of data within a program. The input component involves receiving data or information from external sources, such as user input, files, or ==databases==, and storing it in variables for processing. Processing involves performing operations on the input data to produce an output, such as calculations, data manipulation, or running algorithms. Output involves returning the processed data to the user or saving it to an external source, such as a file or database.

>[!info] Database
> A structured collection of data that is stored and organized in a way that allows efficient retrieval and manipulation of the data.

```mermaid
graph LR
    A[Input] --> B[Processing]
    B --> C[Output]
```

This flowchart shows the three main components of the IPO model and their relationship to each other. Data is inputted into the program, processed in some way, and then outputted to the user or saved to an external source.

# Concepts

## Displaying Text

Let's apply the IPO model to Python to better understand it. We will start by focusing on the "Output" component. To demonstrate the "Output" part of the IPO model, we will use the print ==function== in Python to display the text "May the Force be with you" on the screen.

Here is the code that demonstrates the use of `print` function to display the text "May the Force be with you" on the screen:
```python
print("May the Force be with you")
```

When this code block is executed, it will output the text "May the Force be with you" on the screen. The print function in Python is used to display text or other values on the screen. It takes one or more ==arguments== inside the parentheses and displays them on the screen. In this case, we have passed the string "May the Force be with you" as an argument to the print function, which will output it on the screen.

> [!info] Function
> A function is a reusable block of code that performs a specific task. Functions help to organize code and make it more modular, which can simplify development and maintenance. For example, the `print()` function in Python is a built-in function that displays text or other values on the screen. It takes one or more arguments inside the parentheses and outputs them on the console.

> [!info] Argument
> An argument is a value or reference that is passed to a function or method. For example, the print() function in Python takes one or more arguments inside the parentheses and displays them on the screen. The arguments can be strings, variables, or expressions. Providing arguments to a function or method allows it to perform a specific task with customizable input values. The number and type of arguments needed by a function or method depend on the implementation of that function or method.

### Chew the Byte
1. Write a program to print out your name.
2. Write a program to print out your name, but use single quotes to surround the text.

## Displaying Numbers

Just like we display text on the screen, we can also display numbers.

```python
print(5)
```

### Chew the Byte
1. Print out different numbers.
2. Print out a number with a decimal point. e.g. 3.14.

## Math

We have seen how to output data to the screen. Let's now look at the "Processing" part of the IPO model in Python. We will demonstrate this by performing ==arithmetic operations== using the arithmetic operators  `+`, `-`, `*` and `/`.
```python
print(2 + 3)
print(3.14 * 2)
print(9 / 3)
```

> [!info] Arithmetic Operator
> In Python, an Arithmetic Operator is a symbol that performs an action on values. For example, the + operator adds two values, the - operator subtracts one value from another, the * operator multiplies two values, and the / operator divides one value by another. These operators can be used with different types of values, such as numbers or strings, to produce a result.


### Chew the Byte
1. Try some more math operations using `+`, `-`, `*` and `/`.
2. Try math on more than 2 numbers.
3. Try math on more than 2 operators. 

## Joining Text

Joining text is the process of joining two or more texts together to form a single, larger text. In Python, we can join texts using the `+` operator. For example:

```python
print("I am" + " " + "Frodo" + " " + "Baggins, and I'm on a quest to destroy the " + "Ring" + ".")
```

The above code is a Python statement that ==concatenates== multiple pieces of text to form a longer sentence, which is then displayed on the screen.

> [!info] Concatenation
> In Python, concatenation is the process of combining multiple pieces of text or data together to form a single piece of text or data. In the context of text, concatenation involves joining two or more pieces of text into one longer piece of text.
> 
> In Python, the `+` operator can be used to concatenate two or more pieces of text (represented as text literals) together. When the `+` operator is used with text, it joins the pieces of text together in the order they are given. For example, `"Hello" + " " + "world"` would concatenate the pieces of text `"Hello"`, `" "`, and `"world"` to produce the longer piece of text `"Hello world"`.

The `print()` function is used to output the final sentence to the screen. It takes one argument, which is the text that needs to be displayed. In this case, the text is generated by concatenating several pieces of text using the + operator.

The pieces of text being concatenated are enclosed in quotes to indicate that they are string literals. The first piece of text is "My name is", followed by a space (represented by the " "), then "John", another space, and finally "Doe". The spaces are needed to separate the different words in the sentence and make it more readable.

The `+` operator is used to concatenate the different pieces of text together. Without the spaces, the sentence would be displayed as "My name isJohnDoe", which would be difficult to read. By including spaces between the words, the sentence becomes more human-readable, and the output becomes "My name is John Doe".

## Chew the Byte
1. Substitute "Frodo" and "Baggins" for your first and last name.
2. Print out 2 more sentences that are randomly split. Here are some suggestions:
	1. "Do. Or do not. There is no try."
	2. "All we have to decide is what to do with the time that is given us."

## Variables

Variables are named storage locations that hold a value, and they can be used to store and manipulate data in a program. For example:

```python
name = "John"
print(name)
```

In this program, the variable name is assigned the value "John" using the ==assignment operator== =. 

> [!info] Assignment Operator
> In programming, an assignment operator is a symbol or operator used to assign a value to a variable. In Python, the = operator is the assignment operator used to assign a value to a variable.
> 
> The syntax for using an assignment operator is straightforward. The variable to which the value is being assigned is placed on the left-hand side of the operator, and the value to be assigned is placed on the right-hand side of the operator. For example, `name = "John"` assigns the text "John" to the variable `name`.


### Chew the Byte
1. Change "John" to your name.
2. Create a new variable called `age` and assign it the value of your age.


## Input

Let's now look at the Input part of the IPO model. We will do this by looking at the `input` function in Python. The input function allows users to provide data to the program at ==runtime==, making the program more versatile and user-friendly. It displays a prompt message, waits for the user to enter a value, and returns it as text. We can then concatenate text to display personalized messages that include the user's input. For example:

> [!info] Runtime
> In programming, "runtime" refers to the period during which a program is being executed or running. In the context of the Input part of the IPO model in Python, "runtime" refers to the time when the program is running and waiting for user input.

```python
name = input("Enter your name: ")
print("Hello, " + name + "!")
```

The code above demonstrates how the `input()` function can be used to receive input from the user at runtime, specifically to get the user's name.

The first line of the code assigns the value entered by the user to the variable name. The `input()` function is used to display a prompt message asking the user to enter their name. When the user enters their name and presses enter, the value they entered is stored in the name variable.

The second line of the code uses string concatenation to create a personalized message that includes the user's input. The message "Hello, " is concatenated with the value of the name variable, which contains the name the user entered, and "!" is added at the end to create a friendly greeting message.

### Chew the Byte

1. Prompt the user for their first name, then their last name. Use the variables `first_name` and `last_name`. Then display `Hello, {first_name} {last_name}` with the values provided by the user.
2. Prompt the user for their name and age. Then display `Hello {name}, you are {age} years old!`

# Byte To Go

### Madlibs Generator

You have been tasked with creating a Madlibs generator program in Python. Your program should ask the user for several inputs such as nouns, adjectives, and verbs, and then generate a silly and humorous story by inserting those inputs into a pre-defined template.

#### Requirements:
- Ask the user to input several words such as nouns, adjectives, and verbs.
- Use the user's inputs to fill in the blanks of a pre-defined Madlibs template.
- Display the completed Madlibs story to the user.

#### Example:
Here's an example Madlibs template:

> "The {noun1} was so {adj1} that it decided to {verb1} all the way to the {noun2}. When it got there, it was {adj2} and decided to {verb2} instead, just like Frodo and Sam on their journey to destroy the Ring. They encountered many {noun3} along the way, but with the help of their friends, they were able to {verb3} the Ring and save Middle Earth from the forces of {noun4}."

And here's what the completed Madlibs story might look like based on the user's inputs:

> 1.  "The pineapple was so spiky that it decided to roll all the way to the moon. When it got there, it was dizzy and decided to moonwalk instead, just like Frodo and Sam on their journey to destroy the Ring. They encountered many unicorns along the way, but with the help of their friends, they were able to burp the Ring and save Middle Earth from the forces of pickles."
> 2. "The sandwich was so delicious that it decided to dance all the way to the beach. When it got there, it was sandy and decided to swim instead, just like Frodo and Sam on their journey to destroy the Ring. They encountered many llamas along the way, but with the help of their friends, they were able to jump the Ring and save Middle Earth from the forces of broccoli."

Your task is to write a Python program that implements this Madlibs generator, following the requirements listed above. Have fun with it and be creative!