# Task8Exception-Handling-for-Data-Programs
Objective
Learn to handle common Python errors and make data-processing programs more reliable when input values are invalid.
Concepts Covered
try and except to handle errors
else to run code when no exception occurs
finally to run cleanup code
Common exceptions such as ValueError and TypeError
Example: Safe Data Conversion
value = input("Enter a number: ")

try:
    number = float(value)
except ValueError:
    print("Invalid input. Please enter a number.")
else:
    print("Converted value:", number)
finally:
    print("Conversion attempt completed.")
Sample Output
For input 25:
Converted value: 25.0
Conversion attempt completed.
For input hello:
Invalid input. Please enter a number.
Conversion attempt completed.
Key Learning
Specific exception handling prevents a program from stopping unexpectedly and helps it process invalid data safely.
