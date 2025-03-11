### **📌 Python Input, Output, and Import**  

#### **📖 Table of Contents**
- [Python Input](#python-input)  
  - [Taking a Single Input](#taking-a-single-input)  
  - [Converting Input Type](#converting-input-type)  
  - [Taking List Elements as Input](#taking-list-elements-as-input)  
- [Python Output](#python-output)  
  - [Print with Default Separator and End](#print-with-default-separator-and-end)  
  - [Print with Custom Separator and End](#print-with-custom-separator-and-end)  
- [Python Import](#python-import)  
  - [Importing a Module](#importing-a-module)  
  - [Importing Specific Functions](#importing-specific-functions)  
  - [Importing with an Alias](#importing-with-an-alias)  
- [Definitions](#definitions)  

---

## **Python Input**  

Python's built-in function `input()` is used to take input from the user.  

### **Taking a Single Input**  
```python
num = input("Enter a Number: ")
print("You entered:", num)
print("Type of input:", type(num))
```
🔹 By default, `input()` returns data as a string.  

### **Converting Input Type**  
```python
num = int(input("Enter a Number: "))
print("You entered:", num)
print("Type of input:", type(num))
```
🔹 We explicitly convert the input string to an integer using `int()`.  

### **Taking List Elements as Input**  

#### **Method 1: Taking Elements One by One**  
```python
size = int(input("Enter the number of elements: "))
my_list = []

for i in range(size):
    element = int(input(f"Enter element {i+1}: "))
    my_list.append(element)

print("The list is:", my_list)
```
🔹 The user enters the number of elements and inputs them one by one.  

#### **Method 2: Using `map()` and `list()`**  
```python
my_list = list(map(int, input("Enter space-separated numbers: ").split()))
print("The list is:", my_list)
```
🔹 This method allows taking multiple inputs in a single line, converting them to integers, and storing them in a list.  

---

## **Python Output**  

Python's built-in function `print()` is used to display output on the screen.  

### **Print with Default Separator and End**  
```python
print("Hello", "World")
print("Python is awesome!")
```
**Output:**  
```
Hello World
Python is awesome!
```
🔹 The default separator between objects is a space `' '`, and the default `end` is a newline `'\n'`.  

### **Print with Custom Separator and End**  
```python
print("Hello", "World", sep=" & ", end=" | ")
print("Python is awesome!")
```
**Output:**  
```
Hello & World | Python is awesome!
```
🔹 The separator (`sep=" & "`) changes the default space between words, and the `end=" | "` replaces the default newline.  

---

## **Python Import**  

The `import` statement is used to bring modules into the Python environment.  

### **Importing a Module**  
```python
import math

print("Square root of 16:", math.sqrt(16))
print("Factorial of 5:", math.factorial(5))
```
🔹 The `math` module provides various mathematical functions.  

### **Importing Specific Functions**  
```python
from math import factorial, gcd

print("Factorial of 5:", factorial(5))
print("GCD of 8 and 12:", gcd(8, 12))
```
🔹 Instead of importing the whole module, we import only specific functions.  

### **Importing with an Alias**  
```python
import math as m

print("Pi value:", m.pi)
print("Cosine of 0:", m.cos(0))
```
🔹 We use `import math as m`, allowing us to use `m.pi` instead of `math.pi`.  

---

## **Definitions**  

📌 **Function**: A block of reusable code that performs a specific task.  

📌 **Module**: A file containing Python code (functions, classes, variables) that can be imported into another Python program.  

📌 **Type Conversion**: The process of converting a value from one data type to another (e.g., from `str` to `int`).  

📌 **List**: A collection of ordered, changeable, and indexed elements in Python, defined using square brackets `[ ]`.  

📌 **Separator (`sep`)**: A parameter in `print()` that specifies how multiple values are separated in the output.  

📌 **End (`end`)**: A parameter in `print()` that defines what to print at the end of the statement instead of a newline.  

📌 **Alias**: An alternative name assigned to a module to make it easier to use in code.  
