In the previous lesson, we've seen mathematical operators and how to write expressions in Python. In Python, the meaning of an operator may change based on the data types of the values next to it. For example, the `+` sign we used to add numbers together can be used to concatenate two or more strings together. Concatenation simply means joining the strings together.

## String Concatenation

```python
first_name = "John"
last_name = "Smith"
full_name = first_name + " " + last_name # "John Smith"
```
We concatenated the string `John` stored in the `first_name` variable with an empty space then joined both to the string `Smith` stored in the variable `last_name`, producing the full name "John Smith".

## String Replication

We can use the `*` operator to replicate a string a specific amount of times. Multiplying a string by an integer will repeat that an string by the number used as an integer. 

```python
user_name = "Amanda"
repeated_user_name = user_name * 3 # "AmandaAmandaAmanda"
```

## Operating on Different Data Types can Cause Errors

It makes sense to do basic arithmetic operations on numbers and to do things like concatenation and replication on strings, but errors will arise if you attempt to do illogical operations, like adding a number to a string. Below are some common errors when trying to use some operators on different data types.

```
"Jackie" + 4
TypeError: Can't convert `int` object to `str` implicitly.
```

```
"Mendez" * "Amedo"
TypeError: Can't multiply sequence by non-int of type `str`
```

```
"Sarah" * 5.5
TypeError: Can't multiply sequence by non-int of type `float`
```
