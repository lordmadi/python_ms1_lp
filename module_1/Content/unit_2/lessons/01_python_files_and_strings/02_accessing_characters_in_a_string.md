Earlier in the course, we learned that strings can be concatenated together using the addition `+` operator. We also learned that we can convert other data types to a string using the `str` function. Now, let's explore some more operations we can perform on strings.

## What Is An Index?

As we learned before, a string is a sequence of characters. We can manipulate that sequence using its index. In programming, an index is a position that references the location of an element in a sequence. In case of a string, the index refers to the position of a given character. Later in the course, we'll learn that indices can also be accessed for a data structure known as `list`. 

Indices start from 0 in Python — and many other programming languages — , indicating the first character. To access a specific character in a string, identify the index (By counting from 0 and up until you reach it) and enclose it in square brackets.

```python
print("Hello"[0]) # H
print("Carpet"[1]) # a
print("Ranger"[5]) # r
```

If you refer to an index that doesn't exist, the program will throw an `IndexError`.

```python
# This  will throw an error because there is no character at index 9.
# The largest index in the string "Hello" is 4.
print("Hello"[9])
```
Result:
```bash
Traceback (most recent call last):
  File "script.py", line 1, in <module>
    print("Hello"[9])
IndexError: string index out of range
```

Additionally, in Python, you can access elements in reverse order by specifying a negative index, where `-1` represents the last character in the string.

```python
print("Banana"[-1]) # a
print("Darth Vader"[-5]) # V
print ("Tea Pot"[-4]) # " "
```
> Notice that in the last `print` statement the empty space between "Tea" and "Pot" is accounted for as part of the string and can be accessed using its index like any other character.

## Strings Immutability

In Python, strings are immutable. Immutable simply means that once a string is created, it can't be modified in a way that alters the order of its characters.

Attempting to change a character by accessing its index and assigning it to a new value will throw a `TypeError`.

```python
coffee_bean_type = "Arabica"
coffee_bean_type[0] = "T"
print(coffee_bean_type)
```
Result:

```bash
Traceback (most recent call last):
  File "script.py", line 3, in <module>
    coffee_bean_type[0] = "T"
TypeError: 'str' object does not support item assignment
```

In the next concept, we'll learn some more operations we can perform on a string. 

## Exercise

Evaluate the following statements and state what will be printed on screen.

- `Online[1]`
- `Calendar[-2]`
- `Energy Pump[6]`
- `"$trongP@ssWord"[-7]`
- `"_"[2]`

