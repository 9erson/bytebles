# Lesson 1 - The IPO Model

## Introduction
Welcome to the Introduction to Python course! We'll discuss the IPO model and how it applies to programming in this lesson.

## IPO Model - Input, Processing, Output
The IPO model is a fundamental concept in programming that describes the flow of data within a program. The model consists of three main components: Input, Processing, and Output.

### Input
The input component is where the program receives data or information from external sources, such as user input, files, or databases. The input data is then stored in variables for processing.

### Processing
The processing component is where the program performs operations on the input data to produce an output. This can include performing calculations, manipulating data, or running algorithms.

### Output
The output component is where the program returns the processed data to the user or saves it to an external source such as a file or database.

To demonstrate how the IPO model works in Python, let's start with the "Output" component.

## Print
In Python, we use the `print()` statement to display text on the screen. Here's an example:


```python
print("Hello World")
```

    Hello World


Now, try to answer the following questions to understand print() better:
1. What happens if you remove the word "print" from the code?
2. What happens if you remove the parentheses () from the code?
3. What happens if you use only one of the parentheses?
4. What happens if you surround the text with single quotes ' instead of double quotes "?
5. What happens if you change the text "Hello World" to another text, like "Hey World"?
6. What happens if you change the text "Hello World" to a number, like 5?
7. What happens if you remove the double quotes and just keep the number, i.e., 5?
We will next look at the "Processing" component of the IPO Model. To demonstrate this component in Python, let's look at two concepts - Variables and Joining Text.

## Variables
In programming, a variable is a named storage location that can hold a value. It is used to store and manipulate data in a program.
For example, in Python, we can assign a text value to a variable called name like this:


```python
name = "John"
print(name)
```

    John


Now, the variable name contains the text value "John", which can be used throughout the program. We can also change the value of the variable during the program's execution. For example:


```python
name = "Mary"
print(name)
```

    Mary


Now, the variable name contains the text value "Mary".
Here's the complete code:


```python
name = "John"
print(name)
name = "Mary"
print(name)
```

    John
    Mary


In the revised example, we use the variable name to store text values. We also demonstrate how to change the value of the variable during the program's execution. By using variables, we can create more dynamic and flexible programs that can store and manipulate different data values.

## Joining Text

Joining text is the process of joining two or more texts together to form a single, larger text. In Python, we can join texts using +.
Here's an example of how we can join texts to create a sentence using variables:


```python
first_name = "Frodo"
last_name = "Baggins"
print("Your first name is " + first_name + ", your last name is " + last_name + ", and your whole name is " + first_name + " " + last_name)
```

    Your first name is Frodo, your last name is Baggins, and your whole name is Frodo Baggins


In the example, we use `+` to join the texts and the variable values together to form a complete sentence. By using this Python feature, we can make more dynamic and flexible programs that can show different things depending on the values of variables.
We will finally look at the "Input" component of the IPO Model. To demonstrate this component in Python, let's look at two concepts - Functions and the Input Function.

## Functions
In programming, a function is a named block of code that performs a specific task. Functions allow you to reuse code and make your programs more organized and modular. Functions represent the IPO model in programming, taking input, processing it, and returning output.
To use a function in Python, you call the function by its name, followed by parentheses that may contain arguments, which are values passed into the function.

### The Goal of Write Programs
The goal of writing computer programs is to provide a useful tool or solution to a problem that can benefit a wide range of people, including non-programmers and non-tech individuals. The idea is to create a program that can automate certain tasks or make them more efficient, thus saving time and effort for the end-users. One of the primary objectives of programming is to make technology accessible to everyone, regardless of their technical expertise. For example, apps on smartphones are designed for users to accomplish various tasks without any programming knowledge.

In Python, the input statement allows end-users to influence the processing and output of the program through their input. With the input function, users can provide data to the program at runtime. The data entered can then be processed by the program, and output can be generated accordingly. This feature allows non-programmers to interact with the program and provide inputs, making the program more versatile and user-friendly. Input statements can be used to create interactive programs, which can be useful in many applications, including games, surveys, and simulations.

### Input Function

In Python, there are built-in functions that are part of the language, such as the print and input functions.
The print function is used to display output on the screen, while the input function is used to get input from the user. The input function displays a prompt message and waits for the user to enter a value, which is then returned as text. Unlike the print function, which just displays output, the input function allows you to save the user input to a variable for later use in your program.
Here's an example of how to use the input function:


```python
name = input("Enter your name: ")
print("Hello, " + name + "!")
```

    Enter your name:  John


    Hello, John!


In this example, we use the input function to get the user's name as input. We display a prompt message asking the user to enter their name. The user then enters their name, which is returned as text and stored in the name variable. We then join some text with the value of the name variable to display a greeting message that includes the user's name.
By using built-in functions like print and input, we can create more interactive programs that can display output and take input from the user. Custom functions can also be defined to perform specific tasks and allow for code reuse, making programs more organized and easier to maintain. We will cover custom functions in a future lesson.

## Running Python Code
When it comes to running Python code, there are two primary ways to do so: interactive mode and running code files. The interactive mode allows you to type in code directly into the Python interpreter, and it will execute the code on the fly. On the other hand, running code files involves creating a separate file that contains Python code, which is saved with a ".py" extension, and executing the code by running that file.

The main similarity between both methods is that they both execute Python code. However, there are some key differences between the two. Interactive mode allows you to test small bits of code quickly and see immediate results, while running code files allows you to create more complex programs and run them repeatedly. Another difference is that code files allow you to save your code for future use, whereas interactive mode does not. Additionally, running code files allows you to debug your code more easily and track errors that may not be apparent in interactive mode.

## Exercise - A Madlib Generator

A MadLib is a word game where the player fills in the blanks of a story with various types of words, such as nouns, verbs, adjectives, and adverbs. The game is played by providing the player with a story that contains blank spaces, with instructions to fill in those blank spaces with words of their choosing based on the prompts given. The end result is a story that is often silly or nonsensical, as it is created using random words chosen by the player.


## Review

- Lesson 1 covered the basic concepts of programming, with a focus on the IPO model.
    - The IPO model stands for Input, Processing, and Output.
    - In programming, this model refers to the process of taking input data, performing some processing on that data, and then producing output data.
- We started by looking at the Output component of the IPO model, using the print function to display text on the screen.
    - We learned that the print function takes a text value and displays it on the screen.
- Furthermore, we then looked at the Variables and Joining Text as part of the "Processing" component of the IPO model.
    - We learned that a variable is a named storage location that can hold a value, and how to use variables to store text values and avoid spelling errors.
    - We also learned how to join text and variable values together to form a complete sentence.
- Next, we looked at the Input component of the IPO model.
    - We learned about the input function, which is used to get input from the user.
    - We also learned how to use join texts to display personalized messages that include the user's input.
- Finally, we briefly introduced the concept of Functions and how they represent the IPO model.
    - We learned that functions are named blocks of code that perform a specific task, and that built-in functions like print and input are part of the Python language.
- Throughout the lesson, we used Python features like print, variables, input, joining text to practice the concepts of the IPO model.
- Overall, Lesson 1 provided a solid foundation for understanding the basic concepts of programming and the IPO model.
    - By mastering these concepts, we can begin to write simple programs and build towards more complex projects.
