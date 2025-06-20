## Question:

#### Given an integer `day` denoting the day number, print the corresponding day of the week.

* The week starts from **Monday** (`day = 1`)
* For values **less than 1** or **greater than 7**, print **"Invalid"**
* Ensure **only the first letter** of the answer is capitalized (e.g., "Monday", "Invalid")

Use:

* For C++ : `cout <<`
* For Java : `System.out.print()`
* For Python : `print()`
* For JavaScript : `console.log()`

 

## Approach:

This problem involves checking a single integer value against a set of constant values (1 to 7), making it an ideal case for the `match-case` statement in Python 3.10+.

Steps:

1. Accept the integer input `day`.
2. Use `match-case` to check for values from `1` to `7`.
3. Print the corresponding weekday.
4. Use the `_` wildcard to handle out-of-range values as `"Invalid"`.

 

## Solution:

```python
class Solution:
    def whichWeekDay(self, day):
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
