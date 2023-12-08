Up to this point, we've only seen loops that repeat a block of code a certain amount of times before it terminates. In Python, you could also nest loops.

## Nesting Loops In Python

Nesting loops refers to the practice of placing one or more loops inside another loop. This creates a nested or inner loop within the body of an outer loop. Nesting loops is a way to perform more complex iterations and is usually useful when handling multidimensional data structures, as we'll explore later in the course.

Innermost loops finish all their iterations before moving out to the outer loop.

```python
for x in range(3):
    for y in range(2):
        print(x, y)
```
Result:

```
0 0
0 1
1 0
1 1
2 0
2 1
```
In this example, the outer loop initially iterates once and prints the value of `x`, which is 0. Then, the inner loop does all its iterations (from 0 to 1) before it terminates. Once the inner loop terminates, the outer loop iterates again and at the second iteration, the value of `x` is 1, and so on.

This table might help illustrate how the above example works more explicitly.

| Current Outer Loop Iteration | value of `x` | value of `y` |
| ---------------------------- | ------------ | ------------ |
| 1<sup>st<sup>                | 0            | 0            |
| 1<sup>st<sup>                | 0            | 1            |
| 2<sup>nd<sup>                | 1            | 0            |
| 2<sup>nd<sup>                | 1            | 1            |
| 3<sup>rd<sup>                | 2            | 0            |
| 3<sup>rd<sup>                | 2            | 1            |

## Exercise

Refactor the code below to use `while` loops instead of `for` loops.

```python
for x in range(3):
    for y in range(2):
        print(x, y)
```