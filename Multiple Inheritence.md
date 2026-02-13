# Arithmetic Operations Using Multiple Inheritance in Python

This Python program demonstrates **multiple inheritance** by performing basic arithmetic operations — Addition, Subtraction, and Division — using three classes.

## 🎯 Aim

To write a Python program to calculate **Add, Sub & Division** using **Multiple Inheritance**.

## 🧠 Algorithm

1. **Define `Calculation1` class**
   - Contains `Summation(a, b)` method to return the sum of two numbers.
2. **Define `Calculation2` class**
   - Contains `Subtraction(a, b)` method to return the difference of two numbers.
3. **Define `Derived` class**
   - Inherits from both `Calculation1` and `Calculation2`.
   - Contains `Division(a, b)` method to return the division result.
4. **Input**
   - Prompt the user to enter two numbers.
5. **Process**
   - Create an object of the `Derived` class.
   - Call `Summation`, `Subtraction`, and `Division` methods.
6. **Output**
   - Display the results of the three operations.

## 💻 Program 
Add code here
```
class Calculation1:
    def Summation(self, a, b):
        return a + b

class Calculation2:
    def Subtraction(self, a, b):
        return a - b

class Derived(Calculation1, Calculation2):
    def Division(self, a, b):
        if b != 0:
            return a / b
        else:
            return "Cannot divide by zero"

# Input from user
num1 = float(input("Enter first number: "))
num2 = float(input("Enter second number: "))

# Create object of Derived class
obj = Derived()

# Perform operations
print("Addition:", obj.Summation(num1, num2))
print("Subtraction:", obj.Subtraction(num1, num2))
print("Division:", obj.Division(num1, num2))

```
## Output Example
<img width="423" height="265" alt="image" src="https://github.com/user-attachments/assets/1eb600ae-d28d-4bfc-a577-eac1def8df7c" />
### Result
The program successfully demonstrates Multiple Inheritance by combining methods from Calculation1 and Calculation2 in the Derived class. It calculates and displays Addition, Subtraction, and Division of two numbers entered by the user
