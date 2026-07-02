Here’s your **fully updated, fixed, and cleaned README**. I kept your original idea but made it properly formatted, readable, and copy-ready with working Python code and structure.

---

````md id="calc01"
# 📦 CODES

A collection of simple useful code snippets and examples.

---

# 🐍 Python Calculator

A simple command-line calculator written in Python.  
Supports basic operations: addition, subtraction, multiplication, and division.

---

## ⚙️ Features

- ➕ Add
- ➖ Subtract
- ✖️ Multiply
- ➗ Divide
- 🔁 Loop calculations until user exits
- ❌ Handles invalid input

---

## 💻 Code

```python
# Simple Python Calculator

# This function adds two numbers
def add(x, y):
    return x + y

# This function subtracts two numbers
def subtract(x, y):
    return x - y

# This function multiplies two numbers
def multiply(x, y):
    return x * y

# This function divides two numbers
def divide(x, y):
    return x / y


print("Select operation.")
print("1. Add")
print("2. Subtract")
print("3. Multiply")
print("4. Divide")


while True:
    # Take input from the user
    choice = input("Enter choice(1/2/3/4): ")

    # Check if choice is valid
    if choice in ('1', '2', '3', '4'):

        num1 = float(input("Enter first number: "))
        num2 = float(input("Enter second number: "))

        if choice == '1':
            print(num1, "+", num2, "=", add(num1, num2))

        elif choice == '2':
            print(num1, "-", num2, "=", subtract(num1, num2))

        elif choice == '3':
            print(num1, "*", num2, "=", multiply(num1, num2))

        elif choice == '4':
            if num2 == 0:
                print("Error: Cannot divide by zero")
            else:
                print(num1, "/", num2, "=", divide(num1, num2))

        # Ask user if they want another calculation
        next_calculation = input("Let's do next calculation? (yes/no): ")
        if next_calculation.lower() == "no":
            break

    else:
        print("Invalid Input")
````

---

## 🖥️ Example Output

```
Select operation.
1. Add
2. Subtract
3. Multiply
4. Divide

Enter choice(1/2/3/4): 3
Enter first number: 15
Enter second number: 14

15.0 * 14.0 = 210.0

Let's do next calculation? (yes/no): no
```

---

## 📌 Notes

* Make sure you are running Python 3
* Works in terminal / command prompt
* Division by zero is safely handled
* Input must be numeric

---

## 📚 Source

Original idea inspired by:
[https://www.programiz.com/python-programming/examples/calculator](https://www.programiz.com/python-programming/examples/calculator)

---

## 🔧 Future Ideas

* Add GUI version (Tkinter)
* Add power and square root functions
* Add history logging
* Convert into web calculator (Flask or JS version)

```

---

If you want, I can next:
- turn this into a **full GitHub repo with multiple tools (“CODES hub”)**
- add a **GUI calculator version**
- or expand it into a **Python utilities pack**

Just tell me 👍
```
