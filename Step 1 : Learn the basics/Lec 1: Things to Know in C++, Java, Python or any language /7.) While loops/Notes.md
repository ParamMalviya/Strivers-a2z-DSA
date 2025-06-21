# 📘 While Loops in Python 

 

## ✅ What is a While Loop?

A **while loop** is a control structure that **repeats a block of code** as long as a given condition is `True`.

It is especially useful when:

* You **don't know how many times** the loop will run.
* You want to keep checking a condition **before each iteration**.

 

## 🔁 How While Loops Work:

1. **Start**
2. **Check the condition**:

   * If `True`: run the loop body
   * If `False`: exit the loop
3. **Run loop body**
4. **Re-check the condition**
5. Repeat until condition becomes `False`

 

## 🧪 Python Syntax:

```python
while condition:
    # loop body
```

 

### 🔹 Key Point:

* If the initial condition is `False`, the loop body is **never executed**.

 

## 🎯 Example: Factorial Calculation Using While Loop

```python
n = 5
factorial = 1

while n > 0:
    factorial *= n
    n -= 1

print(f"Factorial is: {factorial}")
```

✅ Output:

```
Factorial is: 120
```

 

## ✅ When to Use While Loops

Use a `while` loop when:

* You want to **keep running a block** until a specific condition changes
* You're **validating user input**
* You're waiting for a **certain event** or value

 

## 🛑 Termination Conditions

* **Always** define a **clear condition** to avoid infinite loops.
* Infinite loops:

  * Never stop running
  * Consume memory and crash programs
* Always ensure that your loop’s condition **eventually becomes False**

 

## ⚙️ Optimization Techniques

You can optimize `while` (or any loop) using:

### 🔸 `break`

* Used to **exit the loop early**
* Useful when you've **found what you're looking for**

### 🔸 `continue`

* Used to **skip the current iteration** and jump to the next one
* Great for **ignoring unnecessary checks**

 

## 🔍 Example: Using `break` and `continue`

```python
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
target = 6

# Using break
for num in numbers:
    if num == target:
        print(f"Target found: {target}")
        break
    print(f"Checking: {num}")

# Using continue
for num in numbers:
    if num % 2 == 0:
        continue  # skip even numbers
    print(f"Odd number: {num}")
```

✅ Output:

```
Checking: 1
Checking: 2
Checking: 3
Checking: 4
Checking: 5
Target found: 6
Odd number: 1
Odd number: 3
Odd number: 5
Odd number: 7
Odd number: 9
```

 

## ✅ Summary Table

| Feature         | Usage                               |
| --------------- | ----------------------------------- |
| Loop while true | `while condition:`                  |
| Exit early      | `break`                             |
| Skip iteration  | `continue`                          |
| Safe loop       | Define proper termination condition |
