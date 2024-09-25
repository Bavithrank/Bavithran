# Function to perform addition
def add_numbers(a, b):
    return a + b

# Function to perform subtraction
def subtract_numbers(a, b):
    return a - b

# Function to perform division
def divide_numbers(a, b):
    if b != 0:
        return a / b
    else:
        return "Error: Division by zero is not allowed."

# Main function
def main():
    # Get user input for two numbers
    try:
        num1 = float(input("Enter the first number: "))
        num2 = float(input("Enter the second number: "))

        # Perform addition
        addition = add_numbers(num1, num2)
        print(f"Addition: {num1} + {num2} = {addition}")

        # Perform subtraction
        subtraction = subtract_numbers(num1, num2)
        print(f"Subtraction: {num1} - {num2} = {subtraction}")

        # Perform division
        division = divide_numbers(num1, num2)
        print(f"Division: {num1} / {num2} = {division}")

    except ValueError:
        print("Error: Please enter valid numbers.")

# Run the main function
if __name__ == "__main__":
    main()
