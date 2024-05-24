# Faulty Calculator

This is a simple Python program that performs basic arithmetic operations (addition, subtraction, multiplication, and division). 
However, it has some "faulty" answers for specific inputs as an example of how we can manipulate expected outputs.

## Usage

The program prompts the user to input two numbers and an arithmetic operator (`+`, `-`, `*`, `/`). 

### Specific Faulty Cases

- If the user inputs `56` and `9` with the operator `+`, the program outputs `77` instead of `65`.
- If the user inputs `45` and `3` with the operator `*`, the program outputs `555` instead of `135`.
- If the user inputs `56` and `6` with the operator `/`, the program outputs `4` instead of `9.333...`.

For all other inputs, the calculator performs the standard arithmetic operation correctly.

## Code Explanation

breakdown of the code:

```
# the user for the first number
val1 = int(input("Enter a Number:"))

# the user for the second number
val2 = int(input("Enter 2nd Number"))

# the user for the arithmetic operator
operator = input("Enter A Operator: +,-,*,/")

# Check if the operator is addition
if operator == "+":
    # Check for the specific faulty case
    if val1 == 56 and val2 == 9:
        print("77")  # Deliberately incorrect result
    else:
        print("sum is", val1 + val2)  # Correct addition result

# Check if the operator is multiplication
if operator == "*":
    # Check for the specific faulty case
    if val1 == 45 and val2 == 3:
        print("555")  # Deliberately incorrect result
    else:
        print("multiplication is", val1 * val2)  # Correct multiplication result

# Check if the operator is division
if operator == "/":
    # Check for the specific faulty case
    if val1 == 56 and val2 == 6:
        print("4")  # Deliberately incorrect result
    else:
        print("division is", float(val1 / val2))  # Correct division result

# Check if the operator is subtraction
if operator == "-":
    print("substract is", val1 - val2)  # Correct subtraction result

