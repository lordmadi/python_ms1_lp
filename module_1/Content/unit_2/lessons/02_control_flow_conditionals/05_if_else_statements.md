In the previous concepts, we've learned that we can use comparison and boolean operators to compare values and evaluate expressions to either `True` or `False`. Let's utilize this knowledge to do something useful in Python.

## `if` Statements

In Python, an `if` statement is a control flow statement that allows you to execute a block of code conditionally based on a specified condition. The basic syntax of an if statement looks like this:

```python
if (condition):
    # do something
```

Here, condition is an expression that evaluates to either `True` or `False`. If the condition is `True`, the indented block of code following the if statement will be executed. If the condition is `False`, the code block will be skipped.

```python
x = 1
if (x > 2):
    print(x)
```

In the above example, `print(x)` will not run because the `if` condition `x > 2` evaluates to `False` since `x = 1`. 

## Indentation In Python

In order to write statements like the one in the above example, we indented the `print` statement after we wrote the condition. In Python, indentation is used to define the block of code and indicate the scope of statements within control structures, such as `if` statements and functions. If you wrote code in a different language like JavaScript before, indentation isn't really important as JavaScript uses curly brackets `{}` to indicate a block of code. However, Python uses indentation to determine the grouping of statements.

> By convention, code that belongs to a group of statement should be indented either by 2 or 4 spaces (Usually pressing the `Tab` key will do it for you). Also, identation is done automatically when using a code editor like Visual Studio Code if you break a line after an `if` statement or any other group of statements.

## The Elif/Else Clauses

Sometimes when you write `if` statements, you want the program to do something else when the `if condition` is not met. You can use the `else` clause to acheive this.

```python
print("Please input your age")
user_age = input() # input() return a string in all cases.
if (int(user_age) >= 13):
    print("You are eligible to use our services")
else:
    print("Sorry, you can't use our services")
```
In this block of code, if a user inputs a number less than 13, the `if` condition will not be met and the else condition will be automatically met and whatever code comes after it will be executed.

In some other cases, you might want to evaluate more than one conditions. You can use the `elif` clause to acheive this. `elif` is just an acronym for `else if`.

```python
print("Please enter the amount of children you have:")
user_input = input()
total_children_count = int(user_input)

# If the user has 1 child
if (total_children_count > 0 and total_children_count < 2):
    print("You are eligible for a 10% discount")

# If the user has 2 children
elif(total_children_count > 1 and total_children_count < 3):
    print("You are eligible for a 15% discount")

# If the user has 3 or more children
elif(total_children_count >= 3):
    print("You are eligible for a 20% discount")

# On wrong input, like a negative number
else:
    print("Invalid input. Please enter a number greater than 0.")
```
In this block of code, the message that will be printed depends on which condition will be fulfilled. The program will check the `if` condition first. If the condition is met, the other `elif/else` blocks will be skipped. Otherwise, the program will go one by one through each `elif` condition and see if it is met. If all `elif` conditions aren't met, the `else` block will be executed.

> Notice that the above program doesn't check for bad input like words or numbers with decimals. 

## Exercise

Create a program that takes in a user passphrase as input and checks the following:
- If the passphrase length is less than 8 characters, print `Weak.`.
- If the passphrase length is 8 to 12 characters, print `Medium`.
- If the passphrase length is 12 characters or more, print `Strong`.