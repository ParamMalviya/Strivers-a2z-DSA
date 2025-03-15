# Pattern-3: Right-Angled Number Pyramid in Python

### 📌 **Table of Contents**

1️⃣ **[Introduction](#introduction)**  
2️⃣ **[Algorithm](#algorithm)**  
3️⃣ **[Python Implementation](#python-implementation)**  
4️⃣ **[Output](#output)**  
5️⃣ **[Explanation](#explanation)**  
6️⃣ **[Customization](#customization)**  
7️⃣ **[Conclusion](#conclusion)**  

## **Introduction**
A right-angled number pyramid is a pattern where numbers are printed in an increasing manner, forming a right-angled triangle shape. It is created using **nested `for` loops**, where:
- The **outer loop** controls the number of rows.
- The **inner loop** prints numbers from `1` to the current row number.

---

## **Algorithm**
1. Take an input `N` (height of the pyramid).
2. Use an **outer loop** to iterate through the rows.
3. Inside the outer loop, use an **inner loop** to print numbers from `1` to `i`.
4. Print a newline (`print()`) after each row.

---

## **Python Implementation**
```python
# Function to print a right-angled number pyramid
def pattern3(N):
    for i in range(1, N + 1):  # Outer loop for rows
        for j in range(1, i + 1):  # Inner loop for numbers
            print(j, end=" ")  # Print numbers on the same line
        print()  # Move to the next line

# Example usage
N = 5  # Height of the pyramid
pattern3(N)
```

---

## **Output**
```
1
1 2
1 2 3
1 2 3 4
1 2 3 4 5
```

---

## **Explanation**
- The outer loop (`for i in range(1, N + 1)`) runs `N` times, creating `N` rows.
- The inner loop (`for j in range(1, i + 1)`) runs `i` times per row, printing numbers from `1` to `i`.
- The `print(j, end=" ")` ensures numbers are printed on the same line.
- The `print()` moves to the next line after each row.

---

## **Customization**
We can modify the pattern by:
1. Changing `N` to create a larger or smaller pyramid.
2. Printing different sequences (e.g., all numbers in each row being the row number).
3. Aligning the pyramid differently.

### **Example: Pyramid with Repeated Row Numbers**
```python
# Function to print a right-angled pyramid with repeated row numbers
def pattern_repeated(N):
    for i in range(1, N + 1):
        for j in range(1, i + 1):
            print(i, end=" ")  # Print row number instead of sequence
        print()

# Example usage
pattern_repeated(5)
```

**Output:**
```
1
2 2
3 3 3
4 4 4 4
5 5 5 5 5
```

---

## **Conclusion**
- Nested `for` loops help create structured patterns.
- The `end=""` parameter in `print()` prevents automatic newlines.
- We can customize the pyramid with different numbers, symbols, or alignments.
