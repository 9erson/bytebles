## Introduction
This Python lesson will introduce you to the `List` data type, which allows you to store multiple values within a single variable. You will learn two ways to create lists: defining all elements at initiation and appending values after the variable is created. You will also learn how to access individual items from a list by index. Additionally, you will be introduced to the `for` loop, which is used to iterate over a list and perform a specific action on each item in the list. The lesson includes several examples and exercises to help you practice using lists and for loops. Finally, you will complete a project that allows you to apply what you have learned by creating a Python program that allows the user to enter items for a shopping list.

## The List Data Type

In Python, we have seen variables holding **different** types of data - strings, integers, floats, and booleans. The one thing all these have in common is that the variable only holds **one** piece of data at a time. You could **change** the variable to hold a different value and even a **different** value type, but it will still only be **one** at any given time.

The `List` data type is a **new data type** that allows you to store **multiple** values within a single variable. Lists can be created in three ways: by defining all elements at initiation, by appending values **after** the variable is created, or a combination of the two.
We use **square brackets** `[` and `]` to tell Python that we want to create a list. If we choose to definte the elements at initiation, we all the elements within the square brackets and separate them by a comma.

### Defining All Elements at Initiation

You can create a list with all its elements specified when the variable is created:

```python
names = ["John", "Jane", "Alice"]
print(names) # Output -> ['John', 'Jane', 'Alice']
```

Each item in the list can be of different types. For example, you could create a list of a person's **name**, **age**, **height**, and if the person **is married**.

```python
person1 = ["John", 25, 5.9, False]
person2 = ["Jane", 21, 5.0, True]
print(person1) # Output -> ['John', 25, 5.9, False]
print(person2) # Output -> ['Jane', 21, 5.0, True]
```

### Appending Values After the Variable is Created

Alternatively, you can create an empty list and append values to it after the variable is created:

```python
names = []
names.append("John")
names.append("Jane")
print(names) # Output -> ['John', 'Jane']
```

You can also mix it up and define some values at the time of creation, and append some values later.

```python
nums = [1, 2, 3]
nums.append(4)
nums.append(5)
print(nums) # Output -> [1, 2, 3, 4, 5]
```

### Accessing Particular Items from a List

We can access individual items from a list by index. Note that counting starts from 0. Here is an example:

```python
names = ["John", "Jane", "Alice"]
first_name = names[0]
second_name = names[1]
print(first_name) # John
print(second_name) # Jane
```

Both methods of list creation can be useful depending on the situation. Defining all elements at initiation is helpful when you already know the data to be stored, while appending values is particularly useful when you need to build a list dynamically, such as when reading data from a file or collecting user input.

### Chew the Byte
1. Create a list variable called `days_of_the_week`, and assign it with the days of the week (Monday, Tuesday, etc.). Then print out the list.
2. Create a list variable called `sibling_ages`. Start with an empty list, append the current age of you and your siblings, starting with the eldest. Then print out the list.

## The For Loop

If the list has many values, and we want to perform some action on each item in the list, we use the **for loop**. 

> [!For Loop]
> The for loop is used to **iterate** over a list.

Here is an example of how to use the for loop in Python:

```python
names = ["John", "Jane", "Tom", "Sarah", "Rick"]
for name in names:
    print(name)
```

This loop will iterate over the `names` list and print out each name. You can use the for loop to perform a specific action on each item in the list.

Here is another example:

```python
nums = [12, 14, 21, 32]
for num in nums:
    print(num * 2)
```

This loop will iterate over the `nums` list and print out each number multiplied by two.

### Chew the Byte
1. Create a variable called `nums` and assign it a list of integers. Then, using the for loop, print out half of each number.
2. You have a list of names, and you need to collect their ages. Write a program that loops through the list of names, then prompts the user to enter that person's age. Append each age to a variable called `ages`. Finally, print out the `names` variable and the `ages` variable. Here is some starting code:
```python
names = ["Peter", "James", "John"]
ages = []
for name in names:
	# Get the age for 'name' and append it to ages.

# Print out names and ages

```

## Project

Write a Python program that allows the user to enter items for their family's weekly grocery shopping trip. 
1. The program should prompt the user to enter an item, and each time an item is entered, the program should add it to a list and print the entire list. 
2. The program should continue prompting the user for items until the user types enter. 
3. At that point, the program should stop prompting for input and enter a "Thank You" message.

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

## Conclusion

In this Python lesson, we learned about the `List` data type, which allows us to store multiple values within a single variable. We learned how to create lists by defining all elements at initiation, appending values after the variable is created, or a combination of the two. We also learned how to access individual items from a list by index and how to use the `for` loop to iterate over a list and perform a specific action on each item in the list. We practiced using lists and for loops through several examples and exercises. Finally, we applied what we learned by creating a Python program that allows the user to enter items for a shopping list. With these skills, we can create powerful programs to manipulate and analyze data in Python.