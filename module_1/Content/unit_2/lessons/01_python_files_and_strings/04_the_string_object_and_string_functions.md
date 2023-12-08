When we explored some built-in functions like `len` and `str`. In `len`, we passed in input directly within the function parentheses (like `len("Hello")`). There is another kind of functions known as a "method". Such functions belong to and are accessible only by a specific object. So, what is an object?

## Objects In Python

In Python, an object is a fundamental concept representing a piece of data, along with the methods or functions that can be applied to that data. Everything in Python is an object, and each object has a specific type (class) that defines its behavior.

For instance, all strings we can write in a program belong to the `String` object. All strings inherit common properties and methods from the `String` object.

For instance, all strings share some common properties like:
- They are immutable.
- Characters in strings can be accessed via index.

Object methods (functions) can be accessed using the `dot` notation, following this syntax:

```python
<Object_Name>.method()
```
> We'll explore Python objects and classes in a greater detail later in the course.

Below, we'll explore three methods that we can use on all strings.

## The `upper` Function

This method takes a string and returns it in uppercase.

```python
fruit = "peach"
model = "AIRbus"
print(fruit.upper()) # PEACH
print(model.upper()) # AIRBUS
```

## The `lower` Function

This method takes a string and returns it in lowercase.

```python
animal = "CAT"
app_name = "Cool Video Editor"
print(animal.lower()) # cat
print(app_name.lower()) # cool video editor
```

## The `title` function

This method takes a string and returns it in title case. In title case, the first character of each word is capitalized while the rest of the characters are lowercase.

```python
day = "friday"
course_name = "data structures"
favorite_drink = "CARAMEL latte"
print(day.title()) # Friday
print(course_name.title()) # Data Structures
print(favorite_drink.title()) # Caramel Latte
```