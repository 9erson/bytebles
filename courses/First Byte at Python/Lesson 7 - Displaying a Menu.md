
## Print list of items
```python
items = ["Red", "Green", "Blue"]

for item in items:
    print(item)
```

### Exercises
1. Create a list of days of the week, then print them - one on each line.
2. Create a list of names. Then on each line, greet each person from the list ("Hello John", "Hello Jane", etc.)

## Print numbered list of items

```python
items = ["Red", "Green", "Blue"]

for index, item in enumerate(items):
    print(f"{index + 1}. {item}")
```

### Exercises
1. Create a list of months of the year, then print a numbered list - one on each line.
2. Create a list name of your siblings in order of age, oldest first. Then print a numbered list, one on each line. 

## Pick from a list of items
```python
items = ["Red", "Green", "Blue"]

print("Pick an item:")
for index, item in enumerate(items):
    print(f"{index + 1}. {item}")

choice = int(input("Choice: "))

if choice <= len(items):
    print(f"You picked: {items[choice - 1]}")
else:
    print(f"Invalid choice: {choice}")
```

### Exercises
1. Create a list of items on a restaurant menu. Display it as a numbered list and ask the user to pick an item. Then display the message - "You picked Fries!"
2. Create a list of names of people. Display the names as a numbered list and ask to user to pick a name. Then print out the number of characters the name has.

## Add item to list
