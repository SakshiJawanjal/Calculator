# Calculator 
It is a simple calculator with basic arithmetic operation 
Author:Sakshi Jawanjal 

# Prompt the user to enter two numbers
num1 = float(input("Enter the first number: "))
num2 = float(input("Enter the second number: "))

# Display operation choices
print("\nChoose an operation:")
print("1. Addition (+)")
print("2. Subtraction (-)")
print("3. Multiplication (*)")
print("4. Division (/)")

# Get the user's choice
choice = input("\nEnter the number corresponding to your choice (1/2/3/4): ")

# Perform the chosen operation
if choice == '1':
    result = num1 + num2
    operation = "Addition"
elif choice == '2':
    result = num1 - num2
    operation = "Subtraction"
elif choice == '3':
    result = num1 * num2
    operation = "Multiplication"
elif choice == '4':
    if num2 != 0:
        result = num1 / num2
        operation = "Division"
    else:
        result = "undefined (division by zero)"
        operation = "Division"
else:
    result = "Invalid choice"
    operation = "None"

# Display the result
print(f"\nOperation: {operation}")
print(f"Result: {result}")
