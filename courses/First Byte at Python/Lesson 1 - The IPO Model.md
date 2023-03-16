# Introduction to Python and IPO Model

Welcome to the Introduction to Python course, where we will discuss the IPO model and its application to programming. The IPO model is a fundamental concept in programming that describes the flow of data within a program. The model consists of three main components: Input, Processing, and Output. In this lesson, we will discuss these components and their implementation in Python.

>[!info] Program
> A set of instructions written in a programming language that a computer can interpret and execute to perform a specific task or solve a problem.


# IPO Model - Input, Processing, Output

The IPO model describes the flow of data within a program. The input component involves receiving data or information from external sources, such as user input, files, or databases, and storing it in variables for processing. Processing involves performing operations on the input data to produce an output, such as calculations, data manipulation, or running algorithms. Output involves returning the processed data to the user or saving it to an external source, such as a file or database.

>[!info] Database
> A structured collection of data that is stored and organized in a way that allows efficient retrieval and manipulation of the data.

>[!info] User input
> Any data or information entered by the user of a program or system that is used as input for processing. Examples of user input include mouse clicks, keyboard entries, and touchscreen gestures. For now, we will only be looking at keyboard entries as user input.


```mermaid
graph LR
    A[Input] --> B[Processing]
    B --> C[Output]
```

This flowchart shows the three main components of the IPO model and their relationship to each other. Data is inputted into the program, processed in some way, and then outputted to the user or saved to an external source.

# Examples

## Output
Now let's try an apply the IPO model to Python. To demonstrate the Output part of the IPO model in Python, we will be using the `print` function to display the text "Hello World" to the screen.

```python
print("Hello World")
```


## Processing

### Variables

Variables are named storage locations that hold a value, and they can be used to store and manipulate data in a program. For example:


```python
name = "John"
print(name)
```

This code will display "John" on the screen. By using variables, we can create more dynamic and flexible programs that can store and manipulate different data values.

### Joining Text

Joining text is the process of joining two or more texts together to form a single, larger text. In Python, we can join texts using +. For example:

```python
first_name = "John"
last_name = "Doe"
print("My name is " + first_name + " " + last_name)
```

This code will display "My name is John Doe" on the screen. By using this Python feature, we can make more dynamic and flexible programs that can show different things depending on the values of variables.

## Input

### Using input() in Python

The input function allows users to provide data to the program at runtime, making the program more versatile and user-friendly. It displays a prompt message, waits for the user to enter a value, and returns it as text. We can join text to display personalized messages that include the user's input. For example:


```python
name = input("Enter your name: ")
print("Hello, " + name + "!")
```

This code will prompt the user to enter their name, and then display "Hello, [name]!" on the screen.

## Exercise

### Madlibs Generator

You have been tasked with creating a Madlibs generator program in Python. Your program should ask the user for several inputs such as nouns, adjectives, and verbs, and then generate a silly and humorous story by inserting those inputs into a pre-defined template.

#### Requirements:
- Ask the user to input several words such as nouns, adjectives, and verbs.
- Use the user's inputs to fill in the blanks of a pre-defined Madlibs template.
- Display the completed Madlibs story to the user.

#### Example:
Here's an example Madlibs template:

> "The {noun1} was so {adj1} that it decided to {verb1} all the way to the {noun2}. When it got there, it was {adj2} and decided to {verb2} instead."

And here's what the completed Madlibs story might look like based on the user's inputs:

> "The pizza was so cheesy that it decided to dance all the way to the moon. When it got there, it was exhausted and decided to sing instead."

Your task is to write a Python program that implements this Madlibs generator, following the requirements listed above. Have fun with it and be creative!