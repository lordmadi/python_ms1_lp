In the previous lesson, we've learned how to write programs that can execute some statements and skip others based on a specific condition or a set of conditions. But, what if we want to repeat some code for a specified amount of times? How do we get the computer to to do this for us?

## Loops In Programming

A loop is a control flow structure that allows a set of instructions to be repeated multiple times. It enables the execution of a block of code repeatedly until a certain condition is met or for a specified number of iterations. Loops are fundamental constructs in programming and are used to automate repetitive tasks, making code more efficient and concise.

Loops are powerful tools for handling repetitive tasks, such as iterating over characters in a string, elements in a list, processing data, or implementing features that require repeated execution of a set of instructions. 

## While Loops

A `while` loop is one kind of loops available in Python. It executes a block of statements repeatedly as long as a specific condition is met. Once a condition becomes `False`, the loop exits. 

```python
x = 3
while (x > 0):
    print(x)
    x = x - 1
```
Result:
```
3
2
1
```

Let's dissect the above code step by step:

- In the first iteration, `x = 3` and the condition `x > 0` will be `True`. `x` will be printed and then x will be decremented by 1. At this point, `x = 2`.
- In the second iteration, `x = 2` and the condition `x > 0` will be `True`. `x` will be printed and then x will be decremented by 1. At this point, `x = 1`.
- In the third iteration, `x = 1` and the condition `x > 0` will be `True`. `x` will be printed and then x will be decremented by 1. At this point, `x = 0`.
- In the fourth iteration, `x = 0` and the condition `x > 0` will be `False`. The loop now exits and no further printing or decrementing will happen.


So, for a loop to execute correctly, there are typically three essential components:

- **Initialization**: Initialize the loop control variable(s) you will use in the condition with an initial value before entering the loop. This step is executed only once at the beginning of the loop.
- **Condition**: Specify a condition that determines whether the loop should continue executing or terminate. The loop will continue as long as this condition is true.
- **Iteration**: Include statements or operations inside the loop that update the loop control variable(s) and bring the loop closer to termination. This step ensures that the loop will eventually meet the exit condition.

If any of these components is implemented in a wrong way, the loop might enter an infinite state. That is, the loop keeps running forever until your program crashes because it will eventually run out of memory. This kind of loops is known as **Infinite Loops**.

```python
x = 3
while (x > 0):
    print(x)
```
Result:
```
3
3
3
3
3
3
.
.
.
.
(The program will eventually freeze and crash)
```

The above piece of code will result in an infinite error as we removed the iteration component `x = x - 1` that was essentially bringing the loop closer to termination with each iteration.

## Exercise 

Create a program that uses a `while` loop to traverse the characters in the string `"Potato"` and print each character.