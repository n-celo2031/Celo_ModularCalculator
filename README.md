# Celo_ModularCalculator

# Modular Calculator Mini-Program

def add_numbers(num1, num2):
    return num1 + num2

def subtract_numbers(num1, num2):
    return num1 - num2

def multiply_numbers(num1, num2):
    return num1 * num2

def divide_numbers(num1, num2):
    if num2 == 0:
        return "Cannot divide by zero"
    else:
        return num1 / num2

# Main Program

# 1. Ask the user to enter two numbers
first_num = float(input("Enter first number: "))
second_num = float(input("Enter second number: "))

# 2. Ask the user to choose an operation
print("\nChoose operation:")
print("1. Addition")
print("2. Subtraction")
print("3. Multiplication")
print("4. Division")

choice = input("Enter choice (1/2/3/4): ")

# 3 & 4. Use separate function and Return result
if choice == '1':
    result = add_numbers(first_num, second_num)
    print(f"\nResult: {first_num} + {second_num} = {result}")

elif choice == '2':
    result = subtract_numbers(first_num, second_num)
    print(f"\nResult: {first_num} - {second_num} = {result}")

elif choice == '3':
    result = multiply_numbers(first_num, second_num)
    print(f"\nResult: {first_num} * {second_num} = {result}")

elif choice == '4':
    result = divide_numbers(first_num, second_num)
    print(f"\nResult: {first_num} / {second_num} = {result}")

else:
    print("\nInvalid choice selected.")
