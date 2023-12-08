In the previous concept, we've seen that a computer may carry out some instructions and/or skip some based on a specific condition or a set of conditions. Programmers use **comparison operators** when the condition depends on comparing two values.

## Comparison Operators In Python

| Operator | Verb                  |
| -------- | --------------------- |
| `==`     | Equal to              |
| `!=`     | Not Equal To          |
| `>`      | Greater than          |
| `>=`     | Greater Than Or Equal |
| `<`      | Less than             |
| `<=`     | Less Than Or Equal    |

> Notice that we use 2 equal signs `==` to compare if two values are equal in Python.

Comparing values using these operators has only two possible results, which are `True` and `False`. But, what are these?

## Boolean Literals In Python

In Python, `True` and `False` are the two Boolean literals representing the state of something whether its true or false, respectively. These values are used in expressions, conditions, and control flow statements to make decisions and perform logical operations.

`True`: Used to indicate that a certain condition or expression is true.

`False`: Used to indicate that a certain condition or expression is false.

```python
print(45 <= 43) # False
print(22 >= 22) # True
print(51 < 50) # False
print(9 != 10) # True
print("Strawberry" == "strawberry") # False
print("7" == 7) # False. Different data types.
```

> Notice that comparing `Strawberry` to `strawberry` returned false because strings are case-sensitive in Python. 

Also, trying to compare different data types using `>`, `>=`, `<`, and `<=` operators will throw an error.

```python
x = 15
y = "Darth Vader"
print (x < y)
```
Result:
```bash
Traceback (most recent call last):
  File "script.py", line 1, in <module>
    print(15 < "Darth Vader")
TypeError: '<' not supported between instances of 'int' and 'str'
```

In the next concept, we'll explore another type of comparison operators called **Boolean operators**.

## Exercise

Evaluate the following expressions and state whether they are `True` or `False`.

- `32 == "32"`
- `5 == 10`
- `"Banana" != "banana"`
- `5 >= 5.0`
- `15 <= 15.5`
- `9 < "Nine"`
