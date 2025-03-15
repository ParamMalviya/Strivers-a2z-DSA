# Understanding `for` Loops and `print()` in Python

## **1. What is a `for` Loop?**
A `for` loop in Python is used to iterate over a sequence (like a list, tuple, string, or range) and execute a block of code multiple times.

### **Basic Syntax:**
```python
for variable in sequence:
    # Code to execute in each iteration
```

### **Example:**
```python
for i in range(5):
    print(i)
```
**Output:**
```
0
1
2
3
4
```

- `range(5)` generates numbers from **0 to 4** (default start is 0).
- `print(i)` prints each number on a new line.

---
## **2. `range()` Function**
`range(start, stop, step)` generates a sequence of numbers.

### **Examples:**
#### **(a) Default `start` value (0 by default)**
```python
for i in range(5):
    print(i)
```
**Output:**
```
0
1
2
3
4
```
_(Equivalent to `range(0, 5)`)_

#### **(b) Specifying `start` and `stop` values**
```python
for i in range(2, 6):
    print(i)
```
**Output:**
```
2
3
4
5
```

#### **(c) Using `step` to control increments**
```python
for i in range(1, 10, 2):
    print(i)
```
**Output:**
```
1
3
5
7
9
```

#### **(d) Decreasing order using negative `step`**
```python
for i in range(10, 0, -2):
    print(i)
```
**Output:**
```
10
8
6
4
2
```

---
## **3. Nested `for` Loops**
A `for` loop inside another `for` loop is called a **nested loop**.

### **Example: Printing a Square Pattern**
```python
def pattern1(N):
    for i in range(N):  # Outer loop for rows
        for j in range(N):  # Inner loop for columns
            print("* ", end="")
        print()  # Moves to the next line

pattern1(5)
```
**Output:**
```
* * * * *
* * * * *
* * * * *
* * * * *
* * * * *
```
- The **outer loop** runs `N` times (for rows).
- The **inner loop** runs `N` times for each row (for columns).
- `print("* ", end="")` prints stars on the same line.
- `print()` moves to the next line after each row.

---
## **4. `print()` Function and `end` Parameter**
The `print()` function is used to display output.

### **(a) Default `print()` behavior (new line)**
```python
for i in range(5):
    print(i)
```
**Output:**
```
0
1
2
3
4
```

### **(b) Using `end` to print on the same line**
```python
for i in range(5):
    print(i, end=" ")
```
**Output:**
```
0 1 2 3 4
```
- `end=" "` replaces the default newline (`\n`) with a space.

### **(c) Customizing `end`**
#### **Using a comma separator:**
```python
for i in range(5):
    print(i, end=", ")
```
**Output:**
```
0, 1, 2, 3, 4,
```

#### **Using a custom symbol:**
```python
for i in range(5):
    print(i, end=" | ")
```
**Output:**
```
0 | 1 | 2 | 3 | 4 |
```

#### **Printing without spaces or new lines:**
```python
for i in range(5):
    print(i, end="")
```
**Output:**
```
01234
```
- The numbers are printed **without spaces or new lines**.

---
## **5. Conditional Statements Inside `for` Loops**
`if-else` conditions can be used inside loops to execute different actions.

### **Example: Even and Odd Numbers**
```python
for i in range(1, 11):
    if i % 2 == 0:
        print(i, "is Even")
    else:
        print(i, "is Odd")
```
**Output:**
```
1 is Odd
2 is Even
3 is Odd
4 is Even
5 is Odd
6 is Even
7 is Odd
8 is Even
9 is Odd
10 is Even
```

---
## **6. Customizing Loop Increments**
### **Example: Printing every 5th number**
```python
for i in range(1, 26, 5):
    print("i =", i)
```
**Output:**
```
i = 1
i = 6
i = 11
i = 16
i = 21
```
- `i += 5` increases `i` by 5 in each iteration.

---
## **Conclusion**
- `for` loops are used for iterating over sequences.
- `range(start, stop, step)` helps control iteration.
- Nested loops allow working with 2D structures.
- `print()` automatically moves to the next line (`\n`).
- Using `end` in `print()` helps control output formatting.
- `if-else` can be used inside loops for conditional logic.
