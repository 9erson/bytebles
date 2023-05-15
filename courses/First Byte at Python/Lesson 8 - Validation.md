# Concepts
## Validating Strings
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

### Chew the Byte
1. Prompt the user for a number between 10 and 20. If the user types any other number, show a validation message and prompt the user to try again. If the user types a number within the range, display `You typed {num}!`.
2. Prompt the user to enter their canadian province. 
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