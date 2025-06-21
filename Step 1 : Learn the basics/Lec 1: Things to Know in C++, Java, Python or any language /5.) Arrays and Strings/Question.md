### ✅ 1. Arrays

## Question:

#### Complete the function `arrayOperations` to perform basic operations on an array:

* Print the first element
* Print the last element
* Print the length of the array
* Print the array in reverse order

Use:

* For C++: `arr[0]`, `arr[n-1]`, `arr.size()`
* For Java: `arr[0]`, `arr[arr.length-1]`, `arr.length`
* For Python: `arr[0]`, `arr[-1]`, `len(arr)`
* For JavaScript: `arr[0]`, `arr[arr.length-1]`, `arr.length`

 

## Approach:

This task demonstrates how to:

1. Access the first and last elements using index positions.
2. Use the `len()` function to find the size of the array.
3. Reverse the array using slicing.

 

## Solution:

```python
class Solution:
    def arrayOperations(self, arr):
        # Print first element
        print(arr[0])

        # Print last element
        print(arr[-1])

        # Print length of array
        print(len(arr))

        # Print reversed array
        print(arr[::-1])
```

---

### ✅ 2. Strings

## Question:

#### Complete the function `stringOperations` to perform basic string operations:

* Print the length of the string
* Print the string in uppercase
* Print the string in lowercase
* Print the string reversed

Use:

* For Python: `len(s)`, `s.upper()`, `s.lower()`, `s[::-1]`

 

## Approach:

This task demonstrates string manipulation using built-in methods in Python:

1. Use `len()` to get the number of characters.
2. Use `.upper()` and `.lower()` for case conversions.
3. Use slicing to reverse the string.

 

## Solution:

```python
class Solution:
    def stringOperations(self, s):
        # Print length
        print(len(s))

        # Print uppercase
        print(s.upper())

        # Print lowercase
        print(s.lower())

        # Print reversed string
        print(s[::-1])
```
