# project1-for-microit(calculator)
creating a calculator for using python programming we cans use any arithmetic operations 

def add(x, y):
    return x + y

def subtract(x, y):
    return x - y

def multiply(x, y):
    return x * y

def divide(x, y):
    if y == 0:
        return "Error: Division by zero!"
    return x / y

def calculator():
    print("Simple Python Calculator")
    print("Operations: +  -  *  /")

    try:
        num1 = float(input("Enter first number: "))
        op = input("Enter operator (+, -, *, /): ")
        num2 = float(input("Enter second number: "))

        if op == "+":
            result = add(num1, num2)
        elif op == "-":
            result = subtract(num1, num2)
        elif op == "*":
            result = multiply(num1, num2)
        elif op == "/":
            result = divide(num1, num2)
        else:
            result = "Invalid operator"

        print("Result:", result)

    except ValueError:
        print("Invalid input! Please enter numeric values.")

if __name__ == "__main__":
    calculator()
