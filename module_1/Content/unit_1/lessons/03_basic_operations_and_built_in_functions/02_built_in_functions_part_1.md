## Functions in Python

In programming, a function is a re-usable block of code that accomplishes a specific task. A function usually takes in some input, processes it, and returns an output. 

We can categorize functions in Python into two main categories — **built-in** functions and **user-defined** functions. Python comes with a lot of built-in functions that make writing code easier and more straightforward. We'll explore a lot of them as we progress. Also, we'll learn how to define custom functions later in the course.

## The `print` function

The `print` function takes in a value as an input and prints it on screen. 

The `print` function has a specific syntax — The keyword `print`, followed by parentheses. Inside the parentheses, we add the string we want to print.

```python
print("Hello World")
```

## The `input` function

The `input` function waits for the user to type some text on the keyboard and press ENTER/RETURN. When Python interpreter encounters an `input` function, a prompt will show up that allows a user to type on the keyboard. Whatever value the user types will be saved to the `user_input` variable as a string.

```python
print("Please enter your name")
user_input = input()
print("Hello, " + user_input)
```

In the above example, if the user inputs "John Smith" on the keyboard, the program will print `Hello, John Smith` on screen.

## The `len` function

The `len` function takes in a string and returns the count of characters in that string. 

```python
print(len("Hello"))
```
If you enter the above value in the interactive shell, `5` will be printed on the screen since thats the total count of characters in the word `Hello`.

> Note that the values returned by all functions — like the count of characters in case of `len` — can be treated as values and can be passed as input to other functions.

## Exercise

Write a program that takes in the first and last name from a user, save each one in a variable and print a statement that reads "Hello <first_name> <last_name>, welcome to our app!"