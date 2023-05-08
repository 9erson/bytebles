# Introduction
In this lesson, we will learn how to work with lists in Python. Lists are a collection of items that are ordered and changeable. We will cover how to create lists, iterate through them, add and remove items from them. By the end of this lesson, you will be able to create a simple shopping list manager.

# Concepts

## Print list of items
```python
items = ["Red", "Green", "Blue"]

# iterate through the list and print each item
for item in items:
    print(item)
```
### Chew the Byte
1. Create a list of days of the week and print each day on a separate line.
2. Create a list of names, then print a greeting for each person on a separate line.
```
Hello John
Hello Pam
Hello Sam
```

## Print numbered list of items
```python
items = ["Red", "Green", "Blue"]

# iterate through the list and print each item with its index
for index, item in enumerate(items):
    print(f"{index + 1}. {item}")
```

> [!Indexes]
> In Python, **indexes** are used to access specific items in a list. It is important to remember that Python counts indexes starting from **0**, while humans usually count starting from **1**. This means that the first item in the list has an index of 0, the second item has an index of 1, and so on. 
> When working with lists in Python, it is important to keep this in mind and **make adjustments** when translating between the index values used by Python and the values we use to refer to items in the list. 
> For example, if we want to access the first item in the list, we need to use an index of 0 instead of 1. Similarly, if we want to add or remove an item from a specific position in the list, we need to use the correct index value, which may require adding or subtracting 1 to account for the difference in counting between Python and humans.

### Chew the Byte
1. Create a list of months of the year and print each month with its number on a separate line.
2. Create a list of your siblings' names in order of age, the oldest first. Print each name with its number on a separate line.

## Pick from a list of items
```python
items = ["Red", "Green", "Blue"]

# display the list as a numbered list and ask the user to pick an item
print("Pick an item:")
for index, item in enumerate(items):
    print(f"{index + 1}. {item}")

# get the user's choice and display the chosen item
choice = int(input("Choice: "))
print(f"You picked: {items[choice - 1]}")
```
### Chew the Byte
1. Create a list of items on a restaurant menu. Display the menu as a numbered list and ask the user to pick an item. Then display the message. E.g. "You picked Fries!"
2. Create a list of names of people. Display the names as a numbered list and ask the user to pick a name. Then print out the number of characters in the chosen name.

## Add item to list
```python
items = ["Red", "Green", "Blue"]

# iterate through the list and print each item with its index
for index, item in enumerate(items):
    print(f"{index + 1}. {item}")

# ask the user to enter a new item and add it to the list
new_item = input("Enter a new colour: ")
items.append(new_item)

# iterate through the updated list and print each item with its index
for index, item in enumerate(items):
    print(f"{index + 1}. {item}")
```
### Chew the Byte
1. Create a list of 3 countries, then prompt the user to add another country to the list. Then display the entire numbered list.
2. Create a list of 3 breeds of dogs, then prompt the user to add another dog breed to the list. Then display the entire numbered list.

## Remove an item from a list
```python
items = ["Red", "Green", "Blue"]

# display the list as a numbered list and ask the user to pick an item to remove
print("Pick an item:")
for index, item in enumerate(items):
    print(f"{index + 1}. {item}")

# get the user's choice and remove the chosen item from the list
choice = int(input("Choice: "))
items.pop(choice - 1)

# iterate through the updated list and print each item with its index
for index, item in enumerate(items):
    print(f"{index + 1}. {item}")
```
### Chew the Byte
1. Create a list of the planets in our solar system. Prompt the user to remove one planet from the list. Then display the updated list.
2. Create a list of animals. Prompt the user to remove one animal from the list. Then display the updated list.

## Byte to Go
Your parents have asked you to create a shopping list manager to manage the weekly grocery shopping list. 
1. Print a welcome message and display the following options to the user:
    * Add an item to the shopping list
    * Remove an item from the shopping list
    * Quit
2. Write the appropriate code for each option. The program should keep asking the user for choices, add or remove items from the list and display the updated list after every change.
3. When the user finally selects 3 (quit), display the final list and exit the program.

# Conclusion
In conclusion, you have learned how to work with lists in Python, including printing lists, adding and removing items, and selecting items from a list. Practice the exercises and work on the project to solidify your understanding of these concepts. Happy coding!