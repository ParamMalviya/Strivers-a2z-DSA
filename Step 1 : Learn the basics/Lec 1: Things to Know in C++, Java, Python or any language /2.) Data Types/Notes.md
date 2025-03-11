You're right again! The issue occurs because GitHub **automatically generates section IDs** by:  
1. Converting text to **lowercase**  
2. Removing **emojis and special characters**  
3. Replacing **spaces with hyphens (`-`)**  

## **🔍 Fixing the Issue**
Since GitHub removes the `8️⃣` emoji and processes only the text, the correct link should be:  

**`#8-summary-of-data-types`**  

### **✅ Corrected Table of Contents**  

📖 **Table of Contents**  

1️⃣ **[Numeric Data Types](#1-numeric-data-types)**  
   - [Integer (`int`)](#example-numeric-data-types)  
   - [Floating-point (`float`)](#example-numeric-data-types)  
   - [Complex (`complex`)](#example-numeric-data-types)  

2️⃣ **[Sequence Data Types](#2-sequence-data-types)**  
   - [String (`str`)](#example-sequence-data-types)  
   - [List (`list`)](#example-sequence-data-types)  
   - [Tuple (`tuple`)](#example-sequence-data-types)  

3️⃣ **[Set and Dictionary Data Types](#3-set-and-dictionary-data-types)**  
   - [Set (`set`)](#example-set-and-dictionary)  
   - [Dictionary (`dict`)](#example-set-and-dictionary)  

4️⃣ **[Boolean Data Type](#4-boolean-data-type)**  
   - [Boolean (`bool`)](#example-boolean)  

5️⃣ **[NoneType](#5-nonetype)**  
   - [`None`](#example-nonetype)  

6️⃣ **[Type Conversion](#6-type-conversion)**  
   - [Converting Between Data Types](#example-type-conversion)  
   - [Examples of Type Casting](#example-type-conversion)  

7️⃣ **[Checking Data Types](#7-checking-data-types)**  
   - [Using `type()` Function](#example-checking-data-types)  

8️⃣ **[Summary of Data Types](#8-summary-of-data-types)**  

---

### **🚀 Why This Fix Works?**  
- `8️⃣` is ignored  
- The actual **header ID** becomes `8-summary-of-data-types`  
- Now the link works perfectly in **GitHub README.md**  

Let me know if you need any more refinements! 😊
**Python Data Types**  

Python provides various built-in **data types** to define the type of data stored in a variable. Python is **dynamically typed**, meaning the type is assigned automatically based on the value.  

## **1️⃣ Numeric Data Types**  

| Data Type  | Description |
|------------|-------------|
| `int`      | Integer (whole numbers) |
| `float`    | Decimal numbers |
| `complex`  | Numbers with real and imaginary parts |

### **Example: Numeric Data Types**  
```python
# Integer
a = 10
print("Integer:", a, "| Type:", type(a))

# Floating-point
b = 10.5
print("Float:", b, "| Type:", type(b))

# Complex number
c = 3 + 4j
print("Complex:", c, "| Type:", type(c))
```

---

## **2️⃣ Sequence Data Types**  

| Data Type  | Description |
|------------|-------------|
| `str`      | Collection of characters (text) |
| `list`     | Ordered, mutable collection |
| `tuple`    | Ordered, immutable collection |

### **Example: Sequence Data Types**  
```python
# String
text = "Python"
print("String:", text, "| Type:", type(text))

# List
my_list = [1, 2, 3, "apple"]
print("List:", my_list, "| Type:", type(my_list))

# Tuple
my_tuple = (1, 2, 3, "banana")
print("Tuple:", my_tuple, "| Type:", type(my_tuple))
```

---

## **3️⃣ Set and Dictionary Data Types**  

| Data Type  | Description |
|------------|-------------|
| `set`      | Unordered collection of unique values |
| `dict`     | Key-value pairs |

### **Example: Set and Dictionary**  
```python
# Set
my_set = {1, 2, 3, 3, 4}
print("Set:", my_set, "| Type:", type(my_set))

# Dictionary
my_dict = {"name": "Alice", "age": 25}
print("Dictionary:", my_dict, "| Type:", type(my_dict))
```

---

## **4️⃣ Boolean Data Type**  

| Data Type  | Description |
|------------|-------------|
| `bool`     | Represents `True` or `False` |

### **Example: Boolean**  
```python
x = True
y = False

print("Boolean x:", x, "| Type:", type(x))
print("Boolean y:", y, "| Type:", type(y))
```

---

## **5️⃣ NoneType**  

| Data Type  | Description |
|------------|-------------|
| `NoneType` | Represents the absence of a value (`None`) |

### **Example: NoneType**  
```python
x = None
print("Value:", x, "| Type:", type(x))
```

---

## **6️⃣ Type Conversion**  
Python allows conversion between different data types using **type casting**.

### **Example: Type Conversion**  
```python
# Converting int to float
a = 10
b = float(a)
print("Converted int to float:", b, "| Type:", type(b))

# Converting float to int
c = 10.5
d = int(c)
print("Converted float to int:", d, "| Type:", type(d))

# Converting string to int
num_str = "100"
num = int(num_str)
print("Converted string to int:", num, "| Type:", type(num))

# Converting list to tuple
my_list = [1, 2, 3]
my_tuple = tuple(my_list)
print("Converted list to tuple:", my_tuple, "| Type:", type(my_tuple))
```

---

## **7️⃣ Checking Data Types**  

Use the `type()` function to check the type of a variable.

### **Example: Checking Data Types**  
```python
x = 42
y = "Hello"
z = [1, 2, 3]

print("Type of x:", type(x))
print("Type of y:", type(y))
print("Type of z:", type(z))
```

---

## **📌 Summary of Data Types**  

| **Type**  | **Example** | **Description** |
|-----------|------------|----------------|
| `int`     | `10, -5` | Whole numbers |
| `float`   | `10.5, -3.14` | Decimal numbers |
| `complex` | `3+4j` | Complex numbers |
| `str`     | `"Hello"` | Text (string) |
| `list`    | `[1, 2, 3]` | Ordered, mutable collection |
| `tuple`   | `(1, 2, 3)` | Ordered, immutable collection |
| `set`     | `{1, 2, 3}` | Unordered, unique collection |
| `dict`    | `{"key": "value"}` | Key-value pairs |
| `bool`    | `True, False` | Boolean (true/false) |
| `NoneType`| `None` | Represents "nothing" |
