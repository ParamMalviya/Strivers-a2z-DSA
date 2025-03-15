# Pattern-4: Right-Angled Number Pyramid - II in Python

### 📌 **Table of Contents**
1️⃣ **[Introduction](#introduction)**  
2️⃣ **[Algorithm](#algorithm)**  
3️⃣ **[Python Implementation](#python-implementation)**  
4️⃣ **[Output](#output)**  
5️⃣ **[Explanation](#explanation)**  
6️⃣ **[Customization](#customization)**   
7️⃣ **[Conclusion](#conclusion)**  

## **Introduction**
A **Right-Angled Number Pyramid - II** is a pattern where each row contains the same number repeated multiple times, equal to the row index. It follows a triangular structure and is implemented using **nested `for` loops**.

---

## **Algorithm**
1. Take an input `N` (the number of rows in the pyramid).
2. Use an **outer loop** to iterate through the rows from `1` to `N`.
3. Inside the outer loop, use an **inner loop** to print the row number (`i`) exactly `i` times.
4. Print a newline (`print()`) after each row.

---

## **Python Implementation**
```python
# Function to print Right-Angled Number Pyramid - II
def pattern4(N):
    for i in range(1, N + 1):  # Outer loop for rows
        for j in range(i):  # Inner loop for printing row number i times
            print(i, end=" ")  # Print the current row number
        print()  # Move to the next line

# Example usage
N = 6  # Size of the pyramid
pattern4(N)
```

---

## **Output**
For `N = 3`:
```
1
2 2
3 3 3
```

For `N = 6`:
```
1
2 2
3 3 3
4 4 4 4
5 5 5 5 5
6 6 6 6 6 6
```

---

## **Explanation**
- The **outer loop** (`for i in range(1, N + 1)`) controls the number of rows.
- The **inner loop** (`for j in range(i)`) ensures that the number `i` is printed exactly `i` times.
- The `print(i, end=" ")` prints numbers in the same line, separated by spaces.
- The `print()` at the end of the outer loop moves to a new line after each row.

---

## **Customization**
### **Example: Pyramid with Different Symbols**
```python
# Function to print Right-Angled Pyramid with Symbols
def pattern_symbol(N):
    for i in range(1, N + 1):
        for j in range(i):
            print("#", end=" ")  # Replace numbers with a symbol
        print()

# Example usage
pattern_symbol(4)
```

**Output:**
```
#
# #
# # #
# # # #
```

---

## **Conclusion**
- Nested `for` loops help create structured number patterns.
- `end=" "` prevents automatic newlines, keeping numbers in the same row.
- We can customize the pattern with different numbers, symbols, or spacing.
