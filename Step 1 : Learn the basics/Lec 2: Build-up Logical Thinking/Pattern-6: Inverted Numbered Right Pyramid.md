# Pattern-6: Inverted Numbered Right Pyramid in Python

## **Table of Contents**
1. [Introduction](#introduction)  
2. [Algorithm](#algorithm)  
3. [Python Implementation](#python-implementation)  
4. [Output](#output)  
5. [Explanation](#explanation)  
6. [Customization](#customization)  
7. [Conclusion](#conclusion)  

## **Introduction**
The **Inverted Numbered Right Pyramid** pattern is a variation of the right-angled number pyramid where numbers are printed in decreasing order of rows. The first row contains numbers from `1` to `N`, and each subsequent row reduces by one number.

---

## **Algorithm**
1. Take an input `N` (number of rows).
2. Use an **outer loop** to iterate through `N` rows.
3. Use an **inner loop** to print numbers starting from `1` up to the current row length.
4. Print a newline (`print()`) after each row.

---

## **Python Implementation**
```python
# Function to print the inverted numbered right pyramid
def pattern6(N):
    for i in range(N, 0, -1):  # Outer loop for decreasing rows
        for j in range(1, i + 1):  # Inner loop for printing numbers
            print(j, end=" ")
        print()  # Move to the next line

# Example usage
N = 6  # Size of the pattern
pattern6(N)
```

---

## **Output**
### **For N = 3:**
```
1 2 3
1 2
1
```

### **For N = 6:**
```
1 2 3 4 5 6
1 2 3 4 5
1 2 3 4
1 2 3
1 2
1
```

---

## **Explanation**
- The **outer loop (`for i in range(N, 0, -1)`)** starts from `N` and decrements down to `1`, controlling the number of rows.
- The **inner loop (`for j in range(1, i + 1)`)** prints numbers from `1` to the current row number.
- The `print(j, end=" ")` ensures that numbers are printed in the same row.
- The `print()` moves to the next line after printing each row.

---

## **Customization**
We can modify the pattern by:
1. **Changing `N`** to increase or decrease the number of rows.
2. **Printing numbers in reverse order** (starting from the row’s maximum value down to `1`).
3. **Replacing numbers with characters or symbols.**

### **Example: Reverse Number Order**
```python
# Function to print numbers in reverse order
def pattern_reverse(N):
    for i in range(N, 0, -1):
        for j in range(i, 0, -1):
            print(j, end=" ")
        print()

# Example usage
pattern_reverse(4)
```

**Output:**
```
4 3 2 1
3 2 1
2 1
1
```

---

## **Conclusion**
- Nested loops are useful for printing structured patterns.
- The decrementing outer loop ensures the pyramid shape.
- The inner loop controls the numbers printed in each row.
- The pattern can be easily customized for different designs.
