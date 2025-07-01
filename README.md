#MY FIRST 50 CODES OF PYTHON AS A BEGINNER 

1.PRINT SOMETHING

print("hello ! it's my actual beginner program. don't worry, you've got this")
print("you can use double quotes or singer quotes. both works but prefer to use doubal quotes")

2.BASIC USE OF OPERATORS

a=5  #we don't need to define data type because python is implicit language
b=6  #basic operators as plus, subtract, divide, power

print(a+b)
print(a-b)
print(a/b)
print(a*b)
print(a**b)

3.SWAP TWO NUMBERS WITHOUT USING THIRD VARIABLE

a = 5
b = 3

a = a + b  
b = a - b  
a = a - b  

print("a =", a)
print("b =", b)

4.CHECK WHETHER IT IS EVEN OR ODD

n=int(input("enter a number to check odd-even:"))

if (n % 2 == 0):
    print(f"{n} is an even number")
else:
    print(f"{n} is an odd number")

|OR|

n = int(input("Enter a number to check odd-even: "))
print(f"{n} is an {'even' if n % 2 == 0 else 'odd'} number")

5.FIND THE GREATEST OF TWO NUMBERS

a = int(input("Enter first number: "))
b = int(input("Enter second number: "))

print(f"{'Both numbers are equal' if a == b else f'{a} is greater' if a > b else f'{b} is greater'}")

6.



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
