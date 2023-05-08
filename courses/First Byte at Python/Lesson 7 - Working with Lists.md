# Introduction
In this lesson, we will learn how to work with lists in Python. We will cover how to create, iterate through, add and remove items from lists. By the end of this lesson, you will be able to create a simple shopping list manager.

# Concepts

## Print list of items
```python
items = ["Red", "Green", "Blue"]

for item in items:
    print(item)
```

### Chew the Byte
1. Create a list of days of the week, then print them - one on each line.
2. Create a list of names. Then on each line, greet each person from the list ("Hello John", "Hello Jane", etc.)

## Print numbered list of items

```python
items = ["Red", "Green", "Blue"]

for index, item in enumerate(items):
    print(f"{index + 1}. {item}")
```

### Chew the Byte
1. Create a list of months of the year, then print a numbered list - one on each line.
2. 1.  Create a list of your siblings' names in order of age, oldest first. Then print a numbered list, one on each line.

## Pick from a list of items
```python
items = ["Red", "Green", "Blue"]

print("Pick an item:")
for index, item in enumerate(items):
    print(f"{index + 1}. {item}")

choice = int(input("Choice: "))

print(f"You picked: {items[choice - 1]}")
```

### Chew the Byte
1. Create a list of items on a restaurant menu. Display it as a numbered list and ask the user to pick an item. Then display the message - "You picked Fries!"
2. Create a list of names of people. Display the names as a numbered list and ask to user to pick a name. Then print out the number of characters the name has.

## Add item to list

```python
items = ["Red", "Green", "Blue"]

for index, item in enumerate(items):
    print(f"{index + 1}. {item}")

new_item = input("Enter a new colour: ")
items.append(new_item)

for index, item in enumerate(items):
    print(f"{index + 1}. {item}")
```

### Chew the Byte
1. Create a list of 3 countries, then prompt the user to add another country. Then display the entire numbered list.
2. Create a list of 3 breeds of dogs, then prompt the user to add another dog breed. Then display the entire numbered list.

## Remove an item from a list

```python
items = ["Red", "Green", "Blue"]

print("Pick an item:")
for index, item in enumerate(items):
    print(f"{index + 1}. {item}")

choice = int(input("Choice: "))

items.pop(choice - 1)

# Print updated list
for index, item in enumerate(items):
	print(f"{index + 1}. {item}")

```

### Chew the Byte
1. Create a list of the planets in our solar system. Then prompt the user to remove one planet. Then display the new list.
2. Create a list of animals. Then prompt the user to remove one animal. Then display the new list.

## Byte to Go
Your parents have asked you to create a shopping list manager to manage the weekly grocery shopping list. Print a welcome message, then prompt the user to pick between 3 options:
1. Add an item to the shopping list
2. Remove an item from the shopping list
3. Quit
Write the appropriate code for each category. The program should keep asking the user the choices, and add or remove from the list. When the user finally selects 3 (quit), Display the final list, and exit the program.

# Conclusion
In conclusion, you have learned how to work with lists in Python, including printing lists, adding and removing items, and selecting items from a list. Practice the exercises and work on the project to solidify your understanding of these concepts. Happy coding!