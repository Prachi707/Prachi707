#HEY I'VE MADE THIS BASIC CALCULATOR! LET ME WHAT CAN I IMPROVE!! 
#  Basic Python Calculator

This is a beginner-level calculator built using Python. It handles basic arithmetic operations like:

- Addition
- Subtraction
- Multiplication
- Division
- Power
- Modulo

---

## How It Works

The program asks the user to input two numbers and select an operation. Based on the input, it performs the calculation and prints the result.

---

## Code



print("Hey bro, I am making a calculator and I think you should give it a shot.\n"
      "There are a few options for operations: plus, subtract, divide, multiply, power, modulo (which gives you remainder)\n")

a = int(input("Enter one of the two numbers you want operations on: "))
b = int(input("Enter the second number: "))

c = input("What kind of operation do you want to operate:\n")

try:
    if c == "plus":
        print(f"Sum of {a} and {b} is {a + b}")
    elif c == "subtract":
        d = float(a - b)
        print(f"Subtraction of {a} and {b} is {d}")
    elif c == "divide":
        if b == 0:
            print("Not divisible by zero")
        else:
            d = float(a / b)
            print(f"Division is {d}")
            print(f"Here is integer division of {a} and {b}: {a // b}")
    elif c == "multiply":
        print(f"Multiplication of {a} and {b} is {a * b}")
    elif c == "power":
        print(f"{a} to the power of {b} is {a ** b}")
    elif c == "modulo":
        if b == 0:
            print("Modulo by zero is undefined.")
        else:
            print(f"Remainder of {a} divided by {b} is {a % b}")
    else:
        print("Enter a valid option!")

except Exception as e:
    print("Sorry, we couldn't get your answer :(")
    print(f"ERROR: {e}")
