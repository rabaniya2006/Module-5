# Hierarchical Inheritance in Python

This Python project demonstrates **Hierarchical Inheritance** using a base class `Details` and two derived classes `Employee` and `Patient`. The program collects and displays details for both employees and patients.

## 🎯 Aim

To write a Python program that uses **Hierarchical Inheritance** to input and display **Employee** and **Patient** details.

## 📘 Description

- **Base Class:** `Details`
  - Stores common attributes: `name`, `age`
  - Provides methods: `getName()`, `getAge()`

- **Derived Class 1:** `Employee`
  - Inherits from `Details`
  - Adds: `employee_id`, `department`
  - Method: `getEmployeeDetails()`

- **Derived Class 2:** `Patient`
  - Inherits from `Details`
  - Adds: `patient_id`, `disease`
  - Method: `getPatientDetails()`

## 🧠 Algorithm

1. Create base class `Details` with common attributes.
2. Create `Employee` class extending `Details`, adding employee-specific data.
3. Create `Patient` class extending `Details`, adding patient-specific data.
4. Get user input for employee and patient data.
5. Display collected information using class methods.

## Program
Add code here
```
class Details:
    def __init__(self, name, age):
        self.name = name
        self.age = age
    
    def getName(self):
        return self.name
    
    def getAge(self):
        return self.age

class Employee(Details):
    def __init__(self, name, age, employee_id, department):
        super().__init__(name, age)
        self.employee_id = employee_id
        self.department = department
    
    def getEmployeeDetails(self):
        print("Employee Details:")
        print("Name:", self.getName())
        print("Age:", self.getAge())
        print("Employee ID:", self.employee_id)
        print("Department:", self.department)
        print()

class Patient(Details):
    def __init__(self, name, age, patient_id, disease):
        super().__init__(name, age)
        self.patient_id = patient_id
        self.disease = disease
    
    def getPatientDetails(self):
        print("Patient Details:")
        print("Name:", self.getName())
        print("Age:", self.getAge())
        print("Patient ID:", self.patient_id)
        print("Disease:", self.disease)
        print()

ename = input("Enter Employee Name: ")
eage = int(input("Enter Employee Age: "))
eid = input("Enter Employee ID: ")
edept = input("Enter Department: ")

pname = input("Enter Patient Name: ")
page = int(input("Enter Patient Age: "))
pid = input("Enter Patient ID: ")
pdisease = input("Enter Disease: ")

emp = Employee(ename, eage, eid, edept)
pat = Patient(pname, page, pid, pdisease)

emp.getEmployeeDetails()
pat.getPatientDetails()

```
## Sample Output
<img width="456" height="721" alt="image" src="https://github.com/user-attachments/assets/2d16b164-e82c-4792-bf9a-8bca87984bfe" />

### Result
The program successfully demonstrates Hierarchical Inheritance where Employee and Patient inherit common attributes from Details while adding their own specific details
