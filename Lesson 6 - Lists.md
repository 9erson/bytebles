## The List data type
- We have seen variables holding different types of data - strings, ints, floats and bools.
	- The one thing all these have in common is that the variable only holds one type of data at a time. 
	- You could change the variable to hold a different value and even a different value type, but it will still only be one at any given time.
-  `List` is a new data type that allows you to store multiple values within a single variable:
  ```python
  names = ["John", "Jane"]
  print(names)
```
- Each item in the list is generally the same type, but doesn't have to be.
	- Example:
	  ```python
	  # Set person's name, age, height and if the person is married.
	  person1 = ["John", 25, 5.9, False]
	  person2 = ["Jane", 21, 5.0, True]
	  print(person1) # Output -> ['John', 25, 5.9, False]
```
- We can access individual items from a list by index (note that counting starts from 0):
  ```python
  names = ["John", "Jane"]
  first_name = names[0]
  second_name = names[1]
  print(first_name) # John
  print(second_name) # Jane
```
## The For Loop
- If the list has many values, and we want to perform some action on each item in the list, we use the for loop.
  ```python
  names = ["John", "Jane", "Tom", "Sarah", "Rick"]
  for name in names:
	  print(name)
```
- Here is another example:
  ```python
  nums = [12,14,21,32]
  for num in nums:
	  print(num * 2)
```
## Project
Imagine you're at a virtual grocery store with friends, and you need to create a shared shopping list. How might you create a program that allows everyone to add items to the list? Can you write a Python program that prompts each person to add an item and then displays the updated list for everyone to see?
Here is the starting code:
```python
# Shopping List Creator

# Create an empty list to hold the shopping items
shopping_list = []

# Loop to prompt the user to enter items
while True:
    # Prompt the user to enter an item
    item = input("Enter an item to add to the shopping list (or press enter to quit): ")

    # If the user enters enter, break out of the loop

    # Add the item to the shopping list

    # Display the updated shopping list

print("Thank you for using the Shopping List Creator!")
```
