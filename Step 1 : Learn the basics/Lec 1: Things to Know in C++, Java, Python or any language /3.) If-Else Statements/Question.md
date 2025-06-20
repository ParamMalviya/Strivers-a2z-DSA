## Question:

#### Complete the function `studentGrade` which takes marks as input and prints the corresponding grade based on the following criteria:

* Grade A if marks ≥ 90
* Grade B if marks ≥ 70
* Grade C if marks ≥ 50
* Grade D if marks ≥ 35
* Fail, otherwise

Use:

* For C++ : `cout <<`
* For Java : `System.out.print()`
* For Python : `print()`
* For JavaScript : `console.log()`

 

## Approach:

The idea is to evaluate the input marks using multiple conditions in descending order of priority.

Steps:

1. Accept marks as input from the user.
2. Use `if-elif-else` statements to compare marks and print the appropriate grade.
3. Ensure conditions are checked from highest to lowest to avoid incorrect grading.

 

## Solution:

```python
class Solution:
    def studentGrade(self, marks):
        if marks >= 90:
            print("Grade A")
        elif marks >= 70:
            print("Grade B")
        elif marks >= 50:
            print("Grade C")        
        elif marks >= 35:
            print("Grade D")
        else:
            print("Fail")
```
