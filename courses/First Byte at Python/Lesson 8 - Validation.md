# Concepts

### Date Type
In Python, the `date` type is part of the `datetime` module, which provides classes for manipulating dates and times. The `date` class provides various methods and attributes to work with dates (year, month, and day).

Here's an example of creating a date object:
```python
from datetime import date

# Create a date object with specific year, month, and day
my_date = date(2021, 9, 15)

print(my_date)  # Output: 2021-09-15
```
To get the current date, you can use the `today()` method:
```python
from datetime import date

# Get the current date
current_date = date.today()

print(current_date)  # Output: The current date, e.g., 2023-05-15
```
To parse a date string, you can use the `strptime()` method from the `datetime` class. It takes two arguments: the date string and the format string:
```python
from datetime import datetime

date_string = "15-05-2023"
format_string = "%d-%m-%Y"

parsed_date = datetime.strptime(date_string, format_string)

print(parsed_date)  # Output: 2023-05-15 00:00:00
```

To format a date object as a string, use the `strftime()` method. It takes a format string and returns a formatted version of the date:

```python
from datetime import date

my_date = date(2023, 5, 15)

formatted_date = my_date.strftime("%B %d, %Y")

print(formatted_date)  # Output: May 15, 2023
```

Here are some commonly used format codes:

- `%Y`: Year with century (e.g., 2023)
- `%m`: Month as a zero-padded decimal number (e.g., 05)
- `%d`: Day of the month as a zero-padded decimal number (e.g., 15)
- `%B`: Month as a full name (e.g., May)
- `%b`: Month as an abbreviated name (e.g., May)
- `%A`: Weekday as a full name (e.g., Monday)
- `%a`: Weekday as an abbreviated name (e.g., Mon)

### Chew the Byte
1. Create a variable called `date_of_birth` and set it to your date of birth. Then print it using an appropriate message.
2. Create 

## Validation
### Input shouldn't be blank
```python
# Initial prompt
name = "Enter your name: "

# Validation Check
while not name:
	# "Validation / Try again" message
	print("Name can't be blank. Try again.")
	# Re-prompt
	name = "Enter your name: "
# Proceed after successul entry
print(f"Hello {name}")
```
### String should be a particular length (e.g. 15 characters)
```python
new_password = input("New Password: ")
while len(new_password) < 15:
	print("Password should be at least 15 characters long. Try again.")
	new_password = input("New Password: ")
```
### Number should be greater than 10

```python
num = input("Enter a number greater than 10: ")
while len < 10:
	print("Number should be greater than 10. Try again.")
	new_password = input("Enter a number greater than 10: ")
```

### Chew the Byte
1. Prompt the user for a number between 10 and 20. If the user types any other number, show a validation message and prompt the user to try again. If the user types a number within the range, display `You typed {num}!`.
2. Prompt the user to enter a valid province code. Show an error if the user types in a wrong code. Use this list:
```python
postal_codes = ['AB', 'BC', 'MB', 'NB', 'NL', 'NS', 'NT', 'NU', 'ON', 'PE', 'QC', 'SK', 'YT']
```


# Byte to Go
Design a Python program for a hotel booking system that includes the following features:

1. Prompt the user to input the start and end dates for their stay, ensuring that the dates are in a valid format (YYYY-MM-DD).
2. Allow the user to select a room type (Deluxe Room or Suite) by entering the corresponding number.
3. Allow the user to choose a board type (Bed & Breakfast, Half-Board, or Full-Board) by entering the corresponding number.
4. Calculate the total cost of the stay based on the following pricing structure:
    - Deluxe Room: $200 per night
    - Suite: $350 per night
    - Wifi: $10 per night (free for Deluxe Rooms and Suites with Full-Board)
    - Half-Board: additional $25 per night
    - Full-Board: additional $50 per night
5. Display the total cost for the user's stay.
6. Add validation to ensure that the user inputs are in the correct format and within the allowed options.

The program should be written in Python, and use logical and comparative operators to simplify cost calculations.