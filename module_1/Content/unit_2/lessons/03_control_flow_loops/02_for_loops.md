Another type of a loop that you can write in a Python program is called a `for` loop. 


## For Loops

A `for` loop is usually used for traversing a sequence of characters or elements in a list which with a length that is known beforehand. The advantage of a `for` loop is that you don't need to explicitly define the `Iteration` component we need in `while `loops.

```python
for char in "Hello":
    print(char)
```
Result:
```
H
e
l
l
o
```
If we translate the above code to plain English, it would read: "For each character in the string `Hello`, print this character". The `for` loop will print each letter in the word `Hello` in each step till it reaches the end. The loop knows when to exit since the length of the word `Hello` is already defined.

> The `char` variable here is user-defined and doesn't necessarily need to be called that. 

## Looping Over a Range Of Values

In some situations, you might need your code to loop a specified amount of times without necessarily taking into consideration the length of a string or the number of elements in a list. To do this, you can use the `range` built-in function.

```python
amount_of_times = 3
for x in range(0, amount_of_times):
    print("Hello")
```
Result:
```
Hello
Hello
Hello
```

The above code iterates over the values starting from 0 to 3 (3 not included) and prints the string `Banana` in each iteration.

> In the `range` function, if you are starting from 0, you can omit it from the code.
> 
> i.e: `range(10)` is the same as `range(0,10)`

## Exercise

Write a `for` loop that uses the `range` function to print any string of your choice only for 5 times.