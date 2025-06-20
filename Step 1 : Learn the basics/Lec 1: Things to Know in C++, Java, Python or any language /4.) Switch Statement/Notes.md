## 📘 Switch/Match-Case Statements in Python

 

## ✅ What’s the Difference Between `if-else` and `switch`?

* **`if-else`** is flexible and used for complex or ranged conditions.
* **`switch` (or `match-case` in Python 3.10+)** is better for **multiple exact matches** of a single variable.
* Use `if-else` when conditions involve comparison or logical operations.
* Use `match-case` when you're comparing **one variable** against multiple **fixed values**.

 

## 🔁 Simulating Switch Case in Python 3.10+

Python introduced the `match-case` statement in version **3.10**, which acts like a switch.

### 🎯 Example: Day of the Week

```python
def get_day_name(day):
    match day:
        case 1:
            print("Monday")
        case 2:
            print("Tuesday")
        case 3:
            print("Wednesday")
        case 4:
            print("Thursday")
        case 5:
            print("Friday")
        case 6:
            print("Saturday")
        case 7:
            print("Sunday")
        case _:
            print("Invalid")
```

✅ Output for `day = 4`: `Thursday`

 

## 📌 Key Points About `match-case` (Switch Equivalent in Python)

### 🔹 1. Constant Matching

* The `match` variable is compared with **constant values** using `case`.
* You can also use expressions or ranges.

```python
def test_expression(val):
    match val:
        case 10 + 5:
            print("Matched 15")
        case _:
            print("No match")
```

 

### 🔹 2. Character Matching

```python
def grade_message(grade):
    match grade:
        case 'A':
            print("Excellent!")
        case 'B':
            print("Good!")
        case _:
            print("Not specified.")
```

✅ Output for `'B'`: `Good!`

 

### 🔹 3. `case _` as Default

* The `_` case acts like the `default` in other languages.
* It executes when none of the above cases match.

 

### 🔹 4. No Fall-Through (Unlike C++)

* In Python, **only the matching `case` block runs**.
* No need for a `break` statement as in C++ or Java.
* Prevents bugs caused by fall-through logic.

 

### 🔹 5. No Duplicate Cases

* Python doesn't allow repeated `case` values in the same match block.
* Each `case` should be **unique**.

 

### 🔹 6. Nested Match-Case (Not Recommended)

* You can nest `match` inside another `match`, but it can become complex and hard to maintain.
* Keep match logic **flat and readable**.

```python
def nested_match(x, y):
    match x:
        case 1:
            print("x is 1")
            match y:
                case 1:
                    print("y is 1")
                case _:
                    print("y is not 1")
```

 

## ⚠️ Note for Older Python Versions

* If you're using **Python < 3.10**, use `if-elif-else` blocks instead of match-case.
* Or simulate switch behavior using **dictionaries** (if you're mapping fixed values to actions).
