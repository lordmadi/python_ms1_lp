## The `str` function

Earlier in this lesson, we've seen that trying to add an integer to a string will produce a `TypeError`. To mitigate this issue, we can use the `str` built-in function. This function takes in an integer that we want to convert and changes its data type from integer to string.

```python
converted_age = str(35)
print("Hello, I am John and I am " + converted_age + " years old.")
# Hello, I am John and I am 35 years old.
```

> Notice that we concatenated the substring `Hello, I am John and I am ` with the value stored in `converted_age` and then we concatenated them together with the substring ` years old.`

## The `int` function

You might've guessed this one. The `int` function takes in a suitable string or a float and converts it to an integer.

```python
int("2187") # 2187
int(-9.99) # -9
int("3.14") # 3
```
That being said, if the string can't be converted to an integer, the function will throw an error.

```python
int("Python is fun")
ValueError: invalid literal for int() with base 10: 'Python is fun'
```

## The `float` function

The `float` function will do the opposite of what `int` does. It will take in a suitable string or an integer and converts it to a float.

```python
float("3.14") # 3.14
float(99981) # 99981.0
float("-35") # -35.0
```

## The `type` function

The `type` function takes in a certain piece of data and checks its type.

```python
type("hello") # <class 'str'>
type(15) # <class 'int'>
type(3.14) # <class 'float'>
```

## Exercise

Write a program that takes in 3 numbers as input from a user, add them together and print the result on screen. 

> Hint: You'll have to use the `int` or `float` functions to convert each user input to a number because the `input` function always returns a string.