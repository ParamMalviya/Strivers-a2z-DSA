# 📘If-Else Statements:

&nbsp;


## ✅ What Are Conditional Statements?

Conditional statements allow your code to **make decisions** and execute different blocks based on conditions.

They include:

* `if`: Executes a block only if the condition is `True`.
* `else`: Executes when the `if` condition is `False`.
* `elif` (short for "else if"): Handles multiple conditions.

&nbsp;

## 🧠 Flow of Control

1. If the condition in `if` is **True**, the code block inside it runs.
2. If the condition is **False**, Python checks for `elif` or executes the `else` block.

&nbsp;

## 🧪 Syntax in Python

```python
if condition:
    # Executes if condition is True
elif another_condition:
    # Executes if first condition is False and this one is True
else:
    # Executes if all conditions above are False
```

&nbsp;

## 🎯 Simple Example: Check Adult Status

```python
age = int(input("Enter your age: "))

if age >= 18:
    print("You are an adult.")
else:
    print("You are not an adult.")
```

&nbsp;

✅ **Output (for input 20)**:

```
You are an adult.
```

&nbsp;

## 📊 Example with `elif`: Grade Based on Marks

```python
marks = int(input("Enter your marks: "))

if marks < 25:
    print("Grade: F")
elif marks < 45:
    print("Grade: E")
elif marks < 50:
    print("Grade: D")
elif marks < 60:
    print("Grade: C")
elif marks < 70:
    print("Grade: B")
elif marks <= 100:
    print("Grade: A")
else:
    print("Invalid marks entered.")
```

&nbsp;

✅ This version uses **only upper bounds** for simplification and clarity.

&nbsp;

## 🛠️ Why `elif` is Better Than Multiple `if`s?

* `elif` ensures **only one** block executes once a condition is met.
* Multiple `if` blocks can lead to **unintended logic**, as more than one may execute if conditions overlap.


&nbsp;

## 🧩 Tip: Use Logical Operators in Conditions

* `and`, `or`, `not` can make your condition checks more powerful.

Example:

```python
if age >= 13 and age <= 19:
    print("You are a teenager.")
```

&nbsp;


## 📌 Summary

* Use `if` for checking conditions.
* Use `else` to catch everything else.
* Use `elif` for handling **multiple specific cases**.
* Keep your condition logic simple and readable.

---
