# **Python Data Types**  

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
