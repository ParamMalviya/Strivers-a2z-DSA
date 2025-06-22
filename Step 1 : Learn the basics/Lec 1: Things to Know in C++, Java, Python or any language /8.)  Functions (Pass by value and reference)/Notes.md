# 📘 Functions in Python – Pass by Value vs Pass by Reference

 

## ✅ What is a Function?

* A **function** is a reusable block of code that performs a specific task.
* Functions make code **modular, readable, and reusable**.

### 🔹 Function Syntax in Python:

```python
def function_name(parameters):
    # body
    return result
```

 

## 🧠 Arguments in Python: Value vs Reference

In Python, **everything is an object**, and function arguments are **passed by object reference** (neither pure "pass-by-value" nor pure "pass-by-reference").

Instead, Python uses:

> **"Call by Object Reference"**
> (or "Call by Assignment")

This means:

* If you pass a **mutable object** (e.g., list, dict), it **can be changed** inside the function.
* If you pass an **immutable object** (e.g., int, str, float), it **cannot be changed** inside the function.

 

## 🔄 Pass by Value (with Immutable Types)

Immutable types: `int`, `float`, `str`, `bool`, `tuple`

When you pass them into a function, their values **do not change** outside the function.

### 🔹 Example:

```python
def increment(x):
    x = x + 1
    print("Inside function:", x)

num = 5
increment(num)
print("Outside function:", num)
```

✅ Output:

```
Inside function: 6
Outside function: 5
```

➡️ `num` remains unchanged because integers are immutable.

 

## 🔁 Pass by Reference (with Mutable Types)

Mutable types: `list`, `dict`, `set`, `bytearray`

Changes made to the object **inside the function** will reflect **outside** as well.

### 🔹 Example:

```python
def add_item(my_list):
    my_list.append(4)
    print("Inside function:", my_list)

numbers = [1, 2, 3]
add_item(numbers)
print("Outside function:", numbers)
```

✅ Output:

```
Inside function: [1, 2, 3, 4]
Outside function: [1, 2, 3, 4]
```

➡️ The list is modified globally because it's mutable.

 

## 📌 Summary Table

| Data Type | Mutable | Changes Inside Function Affect Original? |
| --------- | ------- | ---------------------------------------- |
| `int`     | ❌       | No                                       |
| `float`   | ❌       | No                                       |
| `str`     | ❌       | No                                       |
| `list`    | ✅       | Yes                                      |
| `dict`    | ✅       | Yes                                      |
| `set`     | ✅       | Yes                                      |

 

## 💡 Best Practice Tip

If you want to **avoid unintentional modification**, pass a **copy** of a mutable object:

```python
def safe_modify(lst):
    lst = lst.copy()
    lst.append(100)
    return lst
```

Or explicitly specify in the docstring if the function **modifies** its arguments.

 

## 🧪 Real-Life Analogy

* **Pass by value (immutable)**: Like giving someone a photocopy — changes to it don’t affect the original.
* **Pass by reference (mutable)**: Like giving someone your original notebook — any changes they make affect yours too.
