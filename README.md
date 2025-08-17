# Simple Calculator

def calculator():
    print("=== 🧮 Simple Calculator ===")
    
    try:
        # Take input numbers
        num1 = float(input("Enter first number: "))
        num2 = float(input("Enter second number: "))
        
        # Choose operation
        print("\nChoose operation:")
        print("1. Addition (+)")
        print("2. Subtraction (-)")
        print("3. Multiplication (*)")
        print("4. Division (/)")
        
        choice = input("Enter choice (1-4): ")
        
        # Perform calculation
        if choice == "1":
            result = num1 + num2
            print(f"\n✅ Result: {num1} + {num2} = {result}")
        elif choice == "2":
            result = num1 - num2
            print(f"\n✅ Result: {num1} - {num2} = {result}")
        elif choice == "3":
            result = num1 * num2
            print(f"\n✅ Result: {num1} × {num2} = {result}")
        elif choice == "4":
            if num2 != 0:
                result = num1 / num2
                print(f"\n✅ Result: {num1} ÷ {num2} = {result}")
            else:
                print("\n⚠️ Error: Division by zero is not allowed!")
        else:
            print("\n⚠️ Invalid choice! Please enter 1–4.")
    
    except ValueError:
        print("\n⚠️ Invalid input! Please enter numbers only.")

# Run calculator
calculator()
