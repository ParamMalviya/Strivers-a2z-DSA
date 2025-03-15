# Pattern-5: Inverted Right Pyramid in Python

### 📌 **Table of Contents**
1️⃣ **[Introduction](#introduction)**  
2️⃣ **[Algorithm](#algorithm)**  
3️⃣ **[Python Implementation](#python-implementation)**  
4️⃣ **[Output](#output)**  
5️⃣ **[Explanation](#explanation)**  
6️⃣ **[Customization](#customization)**  
7️⃣ **[Conclusion](#conclusion)**  

## **Introduction**
An **Inverted Right Pyramid** is a pattern where the first row contains `N` stars (`*`), and each subsequent row has one less star until only one remains. This pattern follows a **decreasing triangular structure** and is implemented using **nested `for` loops**.

---

## **Algorithm**
1. Take an input `N` (the number of rows in the pyramid).
2. Use an **outer loop** to iterate from `N` to `1`.
3. Inside the outer loop, use an **inner loop** to print stars (`*`) equal to the current row number.
4. Print a newline (`print()`) after each row.

---

## **Python Implementation**
```python
# Function to print Inverted Right Pyramid
def pattern5(N):
    for i in range(N, 0, -1):  # Outer loop for rows (decreasing order)
        for j in range(i):  # Inner loop for printing stars
            print("*", end=" ")  # Print star with space
        print()  # Move to the next line

# Example usage
N = 5  # Size of the pyramid
pattern5(N)
```

---

## **Output**
For `N = 5`:
```
* * * * *
* * * *
* * *
* *
*
```

For `N = 3`:
```
* * *
* *
*
```

---

## **Explanation**
- The **outer loop** (`for i in range(N, 0, -1)`) starts at `N` and decrements until `1`.
- The **inner loop** (`for j in range(i)`) prints `i` stars in each row.
- The `print("*", end=" ")` ensures stars are printed on the same line, separated by spaces.
- The `print()` at the end of the outer loop moves to a new line after each row.

---

## **Customization**
### **Example: Inverted Pyramid with Different Symbols**
```python
# Function to print Inverted Right Pyramid with Symbols
def pattern_symbol(N):
    for i in range(N, 0, -1):
        for j in range(i):
            print("#", end=" ")  # Replace stars with a symbol
        print()

# Example usage
pattern_symbol(4)
```

**Output:**
```
# # # #
# # #
# #
#
```

---

## **Conclusion**
- Nested `for` loops help create structured patterns.
- `end=" "` prevents automatic newlines, keeping stars in the same row.
- We can modify the pattern by changing symbols or row counts.
