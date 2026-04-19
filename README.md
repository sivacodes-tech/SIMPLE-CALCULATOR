# SIMPLE-CALCULATOR
This is my first project named"SIMPLE CALCULATOR" and I think I did a best version of simple calculator and Im working on my future goals
# Simple Python Calculator
def add(x, y): return x + y
def subtract(x, y): return x - y
def multiply(x, y): return x * y
def divide(x, y): return x / y if y != 0 else "Error"

# User Input
choice = input("Select operation (1-4): ")
num1 = float(input("Enter first number: "))
num2 = float(input("Enter second number: "))

# Logic
if choice == '1': print(add(num1, num2))
# ... additional logic for -, *, /
