# Destructor in Python

This project demonstrates how to implement a **destructor** in Python using a simple class.

## 🚀 Overview

The program defines a class `Demo` with:

- A **constructor** `__init__` that initializes an instance variable and prints a message.
- A **destructor** `__del__` that prints a message when the object is destroyed.

## 🧠 Algorithm

1. Define a class named `Demo`.
2. Inside the class, define the `__init__` method:
   - Initialize an instance variable `status` with the value `"Alive"`.
   - Print the value of `status`.
3. Define the `__del__` method:
   - Print a message indicating the object is being destroyed.
4. Outside the class:
   - Create an instance of the `Demo` class.
   - Delete the object using the `del` keyword.
## Program
Add code Here
```
class Demo:
    def __init__(self):
        self.status = "Alive"
        print("Object created. Status is:", self.status)
    
    def __del__(self):
        print("Destructor called. Object is being destroyed.")

# Create an object
obj = Demo()

# Delete the object
del obj

```
## 🧪 Output
<img width="496" height="190" alt="image" src="https://github.com/user-attachments/assets/6e87cd0e-592b-423b-94e1-bed5228696d3" />

## ResulThe program successfully demonstrates a destructor in Python, where the constructor initializes the object and the destructor is called automatically when the object is deletedt


