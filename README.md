python-calculator/ 
├── .gitignore
├── LICENSE
├── README.md
├── calculator.py
└── main.py 

class Calculator:
    def add(self, a, b): return a + b
    def subtract(self, a, b): return a - b
    def multiply(self, a, b): return a * b
    def divide(self, a, b):
        return a / b if b != 0 else "Error: Division by zero"

from calculator import Calculator

def main():
    calc = Calculator()
    ops = {'+': calc.add, '-': calc.subtract, '*': calc.multiply, '/': calc.divide}
    
    while True:
        print("\nOps: +, -, *, / | 'q' to quit")
        choice = input("Select: ")
        if choice.lower() == 'q': break
        
        if choice in ops:
            try:
                num1 = float(input("Num 1: "))
                num2 = float(input("Num 2: "))
                print(f"Result: {ops[choice](num1, num2)}")
            except ValueError:
                print("Error: Enter numbers only.")
        else:
            print("Invalid input.")

if __name__ == "__main__":
    main()

    __pycache__/
*.py[cod]
.env
.venv/

# Simple Python Calculator

A CLI-based calculator demonstrating basic OOP principles.

## Setup
```bash
python main.py
