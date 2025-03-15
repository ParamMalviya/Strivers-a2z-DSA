# Pattern-6: Inverted Numbered Right Pyramid in Python

## **Table of Contents**
1. [Introduction](#introduction)
2. [Algorithm](#algorithm)
3. [Python Implementation](#python-implementation)
4. [Output](#output)
5. [Explanation](#explanation)
6. [Customization](#customization)
7. [Conclusion](#conclusion)

---

## **Introduction**
An **Inverted Numbered Right Pyramid** is a pattern where the first row contains `N` numbers starting from `1`, and each subsequent row has one less number until only `1` remains. This pattern follows a **decreasing triangular structure** and is implemented using **nested `for` loops**.

---

## **Algorithm**
1. Take an input `N` (the number of rows in the pyramid).
2. Use an **outer loop** to iterate from `N` to `1`.
3. Inside the outer loop, use an **inner loop** to print numbers from `1` to the current row number.
4. Print a newline (`print()`) after each row.

---

## **Python Implementation**
```python
# Function to print Inverted Numbered Right Pyramid
def pattern6(N):
    for i in range(N, 0, -1):  # Outer loop for rows (decreasing order)
        for j in range(1, i + 1):  # Inner loop for printing numbers
            print(j, end=" ")  # Print number with space
        print()  # Move to the next line

# Example usage
N = 5  # Size of the pyramid
pattern6(N)
```

---

## **Output**
For `N = 5`:
```
1 2 3 4 5
1 2 3 4
1 2 3
1 2
1
```

For `N = 3`:
```
1 2 3
1 2
1
```

---

## **Explanation**
- The **outer loop** (`for i in range(N, 0, -1)`) starts at `N` and decrements until `1`.
- The **inner loop** (`for j in range(1, i + 1)`) prints numbers from `1` to `i` in each row.
- The `print(j, end=" ")` ensures numbers are printed on the same line, separated by spaces.
- The `print()` at the end of the outer loop moves to a new line after each row.

---

## **Customization**
### **Example: Inverted Pyramid with Different Start Number**
```python
# Function to print Inverted Numbered Right Pyramid starting from a different number
def pattern_custom(N, start):
    for i in range(N, 0, -1):
        for j in range(start, start + i):
            print(j, end=" ")  # Print numbers with a different start value
        print()

# Example usage
pattern_custom(4, 5)
```

**Output:**
```
5 6 7 8
5 6 7
5 6
5
```

---

## **Conclusion**
- Nested `for` loops help create structured patterns.
- `end=" "` prevents automatic newlines, keeping numbers in the same row.
- We can modify the pattern by changing the start number or row counts.
