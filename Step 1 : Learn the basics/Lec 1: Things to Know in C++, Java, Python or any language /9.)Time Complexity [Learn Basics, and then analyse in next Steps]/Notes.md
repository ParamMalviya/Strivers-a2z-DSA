# 📘 Time and Space Complexity – Notes

 

## ✅ Why Learn Time and Space Complexity?

* Multiple solutions can solve the same problem — **complexity** helps us compare which one is better.
* Time and space complexity measure how **efficient** an algorithm is with respect to **input size**.
* Understanding this is critical for **interviews, competitive coding, and real-world performance**.

 

## 🧠 What is Time Complexity?

Time complexity refers to how the **execution time of an algorithm grows** with input size `N`.

It **does not** depend on:

* Machine speed
* Compiler
* Internet/server delays

Instead, it focuses on **how the number of operations scales** as `N` increases.

 

## 🔍 Time Complexity Is Measured Using:

### ✅ **Big O Notation (O)** – Worst case (most common in interviews)

### 🔸 **Theta (Θ)** – Average case

### 🔹 **Omega (Ω)** – Best case

**But in interviews and most practical scenarios, we focus on Big O.**

 

## 🔄 Time Complexity Basics (with Python Equivalents)

| Code Type                       | Time Complexity |
| ------------------------------- | --------------- |
| Simple statement `x = a + b`    | O(1)            |
| Single loop `for i in range(N)` | O(N)            |
| Nested loop                     | O(N²)           |
| Loop with `i *= 2` (doubling)   | O(log N)        |
| Early exit (worst-case loop)    | O(N)            |

 

### 🧪 Examples:

#### 🔹 Example 1 – Linear loop

```python
for i in range(N):
    pass  # O(1)
# ⟶ O(N)
```

#### 🔹 Example 2 – Nested loops

```python
for i in range(N):
    for j in range(N):
        pass
# ⟶ O(N²)
```

#### 🔹 Example 3 – Logarithmic loop

```python
i = 1
while i < N:
    i *= 2
# ⟶ O(log N)
```

#### 🔹 Example 4 – Early exit (worst-case)

```python
for i in range(N):
    if arr[i] == target:
        break
# ⟶ Best case: O(1), Worst case: O(N)
```

 

## ✅ Rules for Time Complexity Calculation

1. **Worst Case Always**

   * Guarantees max time taken
   * Example: Searching in the last index or element not found

2. **Ignore Constant Multipliers**

   * O(3N) ⟶ O(N)
   * O(1000N + 200) ⟶ O(N)

3. **Ignore Lower Order Terms**

   * O(N² + N + 1) ⟶ O(N²)

4. **Manual Counting is impractical**

   * Instead, analyze **loops, nesting, and growth patterns**

 

## 🧠 Common Time Complexities (Ordered by Speed)

| Big O      | Name              | Meaning                                            |
| ---------- | ----------------- | -------------------------------------------------- |
| O(1)       | Constant time     | Independent of input size                          |
| O(log N)   | Logarithmic time  | Input size reduces each step (e.g., binary search) |
| O(N)       | Linear time       | Grows directly with input                          |
| O(N log N) | Linearithmic time | Merge Sort, Heap Sort                              |
| O(N²)      | Quadratic time    | Two nested loops                                   |
| O(2^N)     | Exponential time  | Recursion without memoization                      |
| O(N!)      | Factorial time    | Brute-force permutations                           |

 

## 🧠 Time Limit Rule in CP Platforms

* Most online judges run approx **10⁸ operations per second**.
* If `time limit = 2s`, your code should not exceed **\~2 × 10⁸ operations**.
* Time complexity must be chosen based on input constraints:

  * N ≤ 10⁵ ⟶ O(N log N) is acceptable
  * N ≤ 10³ ⟶ O(N²) is fine

 

## 📦 What is Space Complexity?

Space complexity refers to the **total memory used** by the algorithm as a function of input size `N`.

It includes:

* **Input Space**: memory for input data
* **Auxiliary Space**: additional memory (variables, arrays, stacks)

 

### 🔹 Example:

```python
def add(a, b):
    c = a + b
    return c
# Space complexity: O(1)
```

```python
arr = [0] * N
# Space complexity: O(N)
```

Recursive functions take up **call stack space**:

```python
def fact(n):
    if n == 0:
        return 1
    return n * fact(n - 1)
# Space: O(N) (due to call stack)
```

 

## 🚫 Bad Practice: Mutating Inputs

Although modifying inputs can reduce space, **avoid mutating input variables** unless the interviewer says so.

Example:

```python
# ❌ Not preferred
b = a + b
```

✅ Use a separate variable:

```python
c = a + b  # Safer, better practice
```

 

## ✅ Summary Table

| Concept          | Key Points                                        |
| ---------------- | ------------------------------------------------- |
| Time Complexity  | How fast code runs as input grows                 |
| Space Complexity | How much memory code uses as input grows          |
| Best Practice    | Always calculate **worst-case** time complexity   |
| Optimization Tip | Use `break`, `continue`, avoid unnecessary memory |
