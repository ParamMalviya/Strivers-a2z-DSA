# Pattern-2: Right-Angled Triangle Pattern in Python

### 📌 **Table of Contents**

1️⃣ **[Introduction](#introduction)**  
2️⃣ **[Algorithm](#algorithm)**  
3️⃣ **[Python Implementation](#python-implementation)**  
4️⃣ **[Output](#output)**  
5️⃣ **[Explanation](#explanation)**  
6️⃣ **[Customization](#customization)**  
7️⃣ **[Conclusion](#conclusion)**  

## **Introduction**
A right-angled triangle pattern is a simple star (`*`) pattern where the number of stars increases as we move down each row. It is created using **nested `for` loops**, where:
- The **outer loop** controls the number of rows.
- The **inner loop** controls the number of stars per row.

---

## **Algorithm**
1. Take an input `N` (height of the triangle).
2. Use an **outer loop** to iterate through the rows.
3. Inside the outer loop, use an **inner loop** to print stars (`*`) equal to the row number.
4. Print a newline (`print()`) after each row.

---

## **Python Implementation**
```python
# Function to print a right-angled triangle pattern
def pattern2(N):
    for i in range(1, N + 1):  # Outer loop for rows
        for j in range(i):  # Inner loop for columns
            print("* ", end="")  # Print stars on the same line
        print()  # Move to the next line

# Example usage
N = 5  # Height of the triangle
pattern2(N)
```

---

## **Output**
```
*
* *
* * *
* * * *
* * * * *
```

---

## **Explanation**
- The outer loop (`for i in range(1, N + 1)`) runs `N` times, creating `N` rows.
- The inner loop (`for j in range(i)`) runs `i` times per row, printing `i` stars.
- The `print("* ", end="")` ensures stars are printed in the same row.
- The `print()` moves to the next line after each row.

---

## **Customization**
You can modify the pattern by:
1. Changing `N` to create a larger or smaller triangle.
2. Replacing `*` with another character.
3. Printing numbers instead of stars.

### **Example: Right-Angled Triangle with Numbers**
```python
# Function to print a right-angled triangle pattern with numbers
def pattern_numbers(N):
    for i in range(1, N + 1):
        for j in range(1, i + 1):
            print(j, end=" ")  # Print numbers instead of stars
        print()

# Example usage
pattern_numbers(5)
```

**Output:**
```
1
1 2
1 2 3
1 2 3 4
1 2 3 4 5
```

---

## **Conclusion**
- Nested `for` loops help create structured patterns.
- The `end=""` parameter in `print()` prevents automatic newlines.
- We can customize the triangle with different symbols, numbers, or alignments.
