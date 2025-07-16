# Python-calculator.py
# Building a calculator CLI app

while True:
    print("\n--- Simple Calculator ---")           # Here, if the user needs to exit, the user needs to type exit or quit.
    print("Type 'exit' to quit.")

    num1 = input("Enter first number: ")          # Here the user chooses the first number 
    if num1 == "exit":
        break

    operator = input("Enter operator (+, -, *, /): ")          # Here the user chooses the operator
    if operator == "exit":
        break

    num2 = input("Enter second number: ")                          # Here the user chooses the second number
    if num2 == "exit":
        break

    num1 = float(num1)
    num2 = float(num2)

    if operator == "+":
        print("Result:", num1 + num2)
    elif operator == "-":
        print("Result:", num1 - num2)
    elif operator == "*":
        print("Result:", num1 * num2)
    elif operator == "/":
        if num2 == 0:
            print("Cannot divide by zero!")
        else:
            print("Result:", num1 / num2)
    else:
        print("Invalid operator!")                                  # If the user put the wrong operator invalid operator will be shown to the screen
