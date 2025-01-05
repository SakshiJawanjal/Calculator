# Calculator 
It is a simple calculator with basic arithmetic operation 
Author:Sakshi Jawanjal 

# Taking two numbers as input
first_number = float(input("Enter the first number: "))
second_number = float(input("Enter the second number: "))

# Display operation menu
print("\nSelect an operation:")
 print("1 - Add")
  print("2 - Subtract")
   print("3 - Multiply")
    print("4 - Divide")

# User selects an operation
operation = int(input("\nEnter the operation number (1/2/3/4): "))

# Perform the selected operation
if operation == 1:
    result = first_number + second_number
    print(f"\nThe sum is: {result}")
elif operation == 2:
    result = first_number - second_number
    print(f"\nThe sub is: {result}")
elif operation == 3:
    result = first_number * second_number
    print(f"\nThe multiplication is: {result}")
elif operation == 4:
    if second_number != 0:
        result = first_number / second_number
        print(f"\nThe quotient is: {result}")
    else:
        print("\nError: Cannot divide by zero.")
else:
    print("\nInvalid selection. Please try again.")
