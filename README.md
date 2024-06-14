# Simple-calculator
Step-by-Step Guide
1. Initialize the Project
Create a new directory for your project.
Initialize a Git repository in the directory.
sh
Copy code
mkdir simple-calculator
cd simple-calculator
git init
2. Create the Python Script
Create a file named calculator.py with the following content:

python
Copy code
def add(a, b):
    return a + b

def subtract(a, b):
    return a - b

def multiply(a, b):
    return a * b

def divide(a, b):
    if b == 0:
        return "Error: Division by zero."
    return a / b

def main():
    print("Simple Calculator")
    print("Select operation:")
    print("1. Add")
    print("2. Subtract")
    print("3. Multiply")
    print("4. Divide")

    choice = input("Enter choice(1/2/3/4): ")

    num1 = float(input("Enter first number: "))
    num2 = float(input("Enter second number: "))

    if choice == '1':
        print(f"{num1} + {num2} = {add(num1, num2)}")
    elif choice == '2':
        print(f"{num1} - {num2} = {subtract(num1, num2)}")
    elif choice == '3':
        print(f"{num1} * {num2} = {multiply(num1, num2)}")
    elif choice == '4':
        print(f"{num1} / {num2} = {divide(num1, num2)}")
    else:
        print("Invalid input")

if __name__ == "__main__":
    main()
3. Add and Commit to Git
Add the calculator.py file to the Git staging area.
Commit the changes to the repository.
sh
Copy code
git add calculator.py
git commit -m "Initial commit: Add basic calculator functionality"
4. Make Some Changes
Let's make some changes to the script. For example, add a new operation for calculating the power of a number.

Update calculator.py:

python
Copy code
def add(a, b):
    return a + b

def subtract(a, b):
    return a - b

def multiply(a, b):
    return a * b

def divide(a, b):
    if b == 0:
        return "Error: Division by zero."
    return a / b

def power(a, b):
    return a ** b

def main():
    print("Simple Calculator")
    print("Select operation:")
    print("1. Add")
    print("2. Subtract")
    print("3. Multiply")
    print("4. Divide")
    print("5. Power")

    choice = input("Enter choice(1/2/3/4/5): ")

    num1 = float(input("Enter first number: "))
    num2 = float(input("Enter second number: "))

    if choice == '1':
        print(f"{num1} + {num2} = {add(num1, num2)}")
    elif choice == '2':
        print(f"{num1} - {num2} = {subtract(num1, num2)}")
    elif choice == '3':
        print(f"{num1} * {num2} = {multiply(num1, num2)}")
    elif choice == '4':
        print(f"{num1} / {num2} = {divide(num1, num2)}")
    elif choice == '5':
        print(f"{num1} ^ {num2} = {power(num1, num2)}")
    else:
        print("Invalid input")

if __name__ == "__main__":
    main()
5. Add and Commit the Changes
Add the modified calculator.py file to the Git staging area.
Commit the changes to the repository.
sh
Copy code
git add calculator.py
git commit -m "Add power operation to calculator"
6. Create a Branch
Create a new branch to add another feature or fix a bug.

sh
Copy code
git checkout -b feature/modulus-operation
7. Add Modulus Operation
Update calculator.py:

python
Copy code
def add(a, b):
    return a + b

def subtract(a, b):
    return a - b

def multiply(a, b):
    return a * b

def divide(a, b):
    if b == 0:
        return "Error: Division by zero."
    return a / b

def power(a, b):
    return a ** b

def modulus(a, b):
    return a % b

def main():
    print("Simple Calculator")
    print("Select operation:")
    print("1. Add")
    print("2. Subtract")
    print("3. Multiply")
    print("4. Divide")
    print("5. Power")
    print("6. Modulus")

    choice = input("Enter choice(1/2/3/4/5/6): ")

    num1 = float(input("Enter first number: "))
    num2 = float(input("Enter second number: "))

    if choice == '1':
        print(f"{num1} + {num2} = {add(num1, num2)}")
    elif choice == '2':
        print(f"{num1} - {num2} = {subtract(num1, num2)}")
    elif choice == '3':
        print(f"{num1} * {num2} = {multiply(num1, num2)}")
    elif choice == '4':
        print(f"{num1} / {num2} = {divide(num1, num2)}")
    elif choice == '5':
        print(f"{num1} ^ {num2} = {power(num1, num2)}")
    elif choice == '6':
        print(f"{num1} % {num2} = {modulus(num1, num2)}")
    else:
        print("Invalid input")

if __name__ == "__main__":
    main()
8. Add and Commit the Changes
Add the modified calculator.py file to the Git staging area.
Commit the changes to the repository.
sh
Copy code
git add calculator.py
git commit -m "Add modulus operation to calculator"
9. Merge the Branch
Switch back to the main branch.
Merge the feature/modulus-operation branch into the main branch.
sh
Copy code
git checkout main
git merge feature/modulus-operation
10. Push to Remote Repository (Optional)
If you have a remote repository (e.g., on GitHub), you can push your changes.

Add the remote repository.
sh
Copy code
git remote add origin https://github.com/yourusername/simple-calculator.git
Push your changes.
sh
Copy code
git push -u origin main