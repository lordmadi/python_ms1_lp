### What Are Variables?

Variables are names given to the data that we need to store and manipulate in a program. Computers store such data by allocating it some storage space in the system memory. 

In more technical terms, program variables are used as **identifiers** that reference the location where the data is stored in the system memory. By doing that, programmers can easily create, change, or delete the stored data whenever needed.

A popular analogy to understand how variables work in a program is the **Box** analogy. In this analogy, let's imagine you are moving out to a new house. You put your items in different boxes and label them so that when you arrive at your new house, you know which box contains what items without the need to open each box and manually check. 

![Python_MS1_Assets_module_1](//images.ctfassets.net/nbtht4kjx2t0/4XCqXOXzB7XtxmpDPrgY9d/8636e40295bc6797182e5bc8b983b672/Python_MS1_Assets__Module_1_.png)

### Creating a Variable

A variable in Python can be any combination of letters (uppercase or lowercase), numbers and underscores, except for the following cases:

- Variables names can't start with a number.
- Variables names can't contain spaces.

Additionally, the following reserved keywords can't be used as variable names in Python:

| False    | def     | if       | raise  |
| -------- | ------- | -------- | ------ |
| None     | del     | import   | return |
| True     | elif    | in       | try    |
| and      | else    | is       | while  |
| as       | except  | lambda   | with   |
| assert   | finally | nonlocal | yield  |
| break    | for     | not      |        |
| class    | from    | or       |        |
| continue | global  | pass     |        |

Let's create some valid variables in Python.

```python
user_name = "John"
age = 25

```

In the above example, we have two variables:

- The `name` variable stores a string called `john`.
- The `age` variable stores an integer `25`.

### The Anatomy of a Variable

Let's dissect what we just provided as an example, bit by bit.

![python_ms1_variable_dissection_module_1](//images.ctfassets.net/nbtht4kjx2t0/7H6eNpRlME6MgRt2K2DUWT/f25e9c84a9ec0c984cd56d95864846a2/Python_MS1_Assets__Module_1___1_.png)

- The variable name `user_name` conforms to the naming rule we mentioned above.
- From its name, the assignment operator `=` is used to assign a certain value to the variable name. Assignment doesn't mean equality. In simpler terms, when we assign a piece of data to a certain variable, we are simply using this variable as a pointer to the location of the memory where that piece of data is stored.
- The data stored `"John"` is a string stored in this variable.

### Variables in Action

A variable —— as the name implies —— can be re-assigned to refer to a different value or even a different data type. For instance:

```python
user_name = "John"
user_name = "Sarah"
```

The variable `user_name` initially stored the string "John", but then the value "John" was replaced by "Sarah". This is called variable re-assignment.

Also, a variable can be used in some programmatic operations. For instance:

```python
user_age = 25
new_user_age = 1 + user_age
print(new_user_age) # 26
```

The variable `new_user_age` stores the result of the addition of the value 1 to the value stored in the variable `user_age`, yielding a result of 26.

Last but not least, a variable can store the value stored in another variable by simply assigning the two names to one another. For instance:

```python
first_name = "Adam"
fname = first_name
```

The variable `fname` is referring to the exact same value stored in the variable `first_name`.

## Adding Code Comments

Python allows programmers to write comments within the lines of code. These comments are useful in cases of debugging —— which is the process of fixing issues with code —— or explaining the functionality of a certain block of code for other programmers to understand. Adding the `#` sign before a line comments it out. If you want to comment out multiple lines at once, enclose them within triple quotes (single or double).

```
# This is a comment and will not be processed by the Python interpreter. 
"""
The code below adds two variables together and saves the result to a third variable
"""
x = 10
y = 15
z = x + y
```

## Exercises

- Create 5 variables that store your name, age, occupation, team members count and department.
- Save the numbers 5, 10, 15 and 20 in variables a, b, c and d, respectively. Then, create two variables; one should store the result of adding all the variables together and the other should store the result of multiplying them.

In the next concepts, we will explore what a string is, how it is different from an integer and what types of data a variable can store.
