# 📘 Arrays & Strings in Python – Notes

 

## ✅ Arrays (Lists in Python)

* Python doesn’t have built-in arrays like C/C++; instead, it uses **lists**.
* Lists can store elements of **any data type** and are **mutable**.

### 🔹 Common Operations:

| Operation            | Code Example                   |
| -------------------- | ------------------------------ |
| Create a list        | `arr = [1, 2, 3, 4]`           |
| Access first element | `arr[0]`                       |
| Access last element  | `arr[-1]`                      |
| Length of list       | `len(arr)`                     |
| Add element          | `arr.append(5)`                |
| Insert at index      | `arr.insert(1, 10)`            |
| Remove by value      | `arr.remove(3)`                |
| Delete by index      | `del arr[2]`                   |
| Reverse list         | `arr[::-1]` or `arr.reverse()` |
| Sort list            | `arr.sort()`                   |

 

## ✅ Strings

* Strings are **immutable** sequences of characters.
* You can access characters using indexing and slicing.
* Strings support many built-in methods for manipulation.

### 🔹 Common Operations:

| Operation               | Code Example          |
| ----------------------- | --------------------- |
| Length of string        | `len(s)`              |
| Convert to uppercase    | `s.upper()`           |
| Convert to lowercase    | `s.lower()`           |
| Reverse a string        | `s[::-1]`             |
| Check substring         | `'abc' in s`          |
| Replace characters      | `s.replace("a", "x")` |
| Find index of substring | `s.find("abc")`       |
| Split into list         | `s.split()`           |
| Join list into string   | `' '.join(words)`     |

 

### 🔑 Tip:

* Strings are **immutable**: operations return a **new string**.
* Lists are **mutable**: operations change the list in place.
