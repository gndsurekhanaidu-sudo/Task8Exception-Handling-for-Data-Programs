# Exception Handling for Data Programs

## Objective
Learn to handle common Python errors using `try`, `except`, `else`, and `finally`.

## Common Exceptions
- `ValueError`: An invalid value is provided, such as `int("hello")`.
- `TypeError`: An operation uses incompatible data types, such as `"10" + 5`.
- `ZeroDivisionError`: A number is divided by zero.
- `IndexError`: An invalid list index is accessed.

## Example: Try-Except
```python
try:
    number = int(input("Enter a number: "))
    print("Number:", number)
except ValueError:
    print("Please enter a valid number")
```

## Data Conversion Program
```python
data = ["10", "20", "hello", "30", "abc"]
numbers = []

for value in data:
    try:
        number = int(value)
        numbers.append(number)
    except ValueError:
        print("Invalid value:", value)

print("Valid numbers:", numbers)
print("Sum =", sum(numbers))
```

### Sample Output
```text
Invalid value: hello
Invalid value: abc
Valid numbers: [10, 20, 30]
Sum = 60
```

## Why Exception Handling Is Important
- Prevents unexpected program termination.
- Handles invalid input safely.
- Makes data-processing programs more reliable.

## Tools
- Python
- Jupyter Notebook

## Conclusion
Exception handling helps a program manage errors and continue processing valid data safely.
