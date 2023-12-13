In some loops, you might face a scenario where you can't control when the loop should terminate, like when you ask a user to input a specific string. In such scenarios, you can't control what the user will input so you might want to keep running the loop till the user inputs the correct information. In Python, there are two useful statements that can help you acheive this.

## The `break` Statement

The `break` statement is used to "break out" of the loop when some external condition is triggered.

```python
while (True):
    print("Please enter your name:")
    user_name = input()
    if (user_name == "Adam"):
        print("Hello Adam, welcome to the app")
        break
```
This program asks the user to input his name. It keeps looping till a user inputs the string `Adam`. If the input is `Adam`, the loop will exit. If the input is anything different from `Adam`, the loop will re-run and the input prompt will show up again.

## The `continue` Statement

The `continue` statement is used to skip the rest of the code inside the loop for the current iteration and proceed to the next iteration. It allows you to bypass certain statements within the loop and move on to the next iteration without executing the remaining code.

```python
for x in range(11):
    if (x % 2 == 0):
        continue
    print(x)
```

This program counts up from 0 to 10. In each iteration, it checks if the number to print is even. If it's even, the loop will skip the execution of the remaining steps (i.e the `print` statement won't execute). Hence, this program only prints odd numbers.

> Remember that `%` is the modulus operator in Python. 

## Exercise

Write a `while` loop that checks if a user enters a number between 1 and 10. Ensure that your code keeps the loop running if the entered number is not in the specified range.
