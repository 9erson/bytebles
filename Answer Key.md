# Lesson 1

# Lesson 4 - Loops


## Print all even numbers between two given numbers.

```python
start_num = 2
end_num = 20

while start_num <= end_num:
    print(start_num)
    start_num += 2
```
## Print the reverse of a given number.

```python
num = 12345
reverse_num = 0

while num > 0:
    remainder = num % 10
    reverse_num = (reverse_num * 10) + remainder
    num = num // 10

```

print(reverse_num)
Generate a Fibonacci sequence up to a given number.
python
Copy code
n = 10
a, b = 0, 1

while a < n:
    print(a)
    a, b = b, a+b
Count the number of digits in a given number.
python
Copy code
num = 12345
count = 0

while num != 0:
    num //= 10
    count += 1

print(count)
Find the largest and smallest digit in a given number.
python
Copy code
num = 12345
largest_digit = num % 10
smallest_digit = num % 10

while num > 0:
    digit = num % 10
    if digit > largest_digit:
        largest_digit = digit
    if digit < smallest_digit:
        smallest_digit = digit
    num //= 10

print("Largest digit:", largest_digit)
print("Smallest digit:", smallest_digit)
I hope this helps! Let me know if you have any questions.