# Pattern-1: Rectangular Star Pattern in Python

### 📌 **Table of Contents**  

1️⃣ **[Introduction](#introduction)**  
2️⃣ **[Algorithm](#algorithm)**  
3️⃣ **[Python Implementation](#python-implementation)**  
4️⃣ **[Output](#output)**  
5️⃣ **[Explanation](#explanation)**  
6️⃣ **[Customization](#customization)**  
   - [Rectangle with Different Rows & Columns](#example-rectangle-with-different-rows-columns)  
7️⃣ **[Conclusion](#conclusion)**  

## **Introduction**
A rectangular star pattern is a simple pattern where we print a matrix of stars (`*`). It is created using **nested `for` loops**, where:
- The **outer loop** controls the number of rows.
- The **inner loop** controls the number of columns.

---

## **Algorithm**
1. Take an input `N` (size of the rectangle, usually square for simplicity).
2. Use an **outer loop** to iterate through the rows.
3. Inside the outer loop, use an **inner loop** to print `N` stars in a row.
4. Print a newline (`print()`) after each row.

---

## **Python Implementation**
```python
# Function to print a rectangular star pattern
def pattern1(N):
    for i in range(N):  # Outer loop for rows
        for j in range(N):  # Inner loop for columns
            print("* ", end="")  # Print stars on the same line
        print()  # Move to the next line

# Example usage
N = 5  # Size of the pattern
pattern1(N)
```

---

## **Output**
```
* * * * *
* * * * *
* * * * *
* * * * *
* * * * *
```

---

## **Explanation**
- The outer loop (`for i in range(N)`) runs `N` times, creating `N` rows.
- The inner loop (`for j in range(N)`) runs `N` times per row, printing `N` stars.
- The `print("* ", end="")` ensures stars are printed in the same row.
- The `print()` moves to the next line after each row.

---

## **Customization**
We can modify the pattern by:
1. Changing `N` to create larger or smaller patterns.
2. Replacing `*` with another character.
3. Adjusting the number of columns independently.

### **Example: Rectangle with Different Rows & Columns**
```python
# Function to print a rectangular star pattern with different rows and columns
def pattern_rect(rows, cols):
    for i in range(rows):
        for j in range(cols):
            print("* ", end="")
        print()

# Example usage
pattern_rect(4, 6)
```

**Output:**
```
* * * * * *
* * * * * *
* * * * * *
* * * * * *
```

---

## **Conclusion**
- Nested `for` loops help create structured patterns.
- The `end=""` parameter in `print()` prevents automatic newlines.
- We can customize the number of rows, columns, and symbols as needed.
