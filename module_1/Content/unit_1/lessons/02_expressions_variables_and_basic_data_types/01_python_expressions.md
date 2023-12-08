## What Is An Expression In Python?

In the previous lesson, we installed and accessed the Python interactive shell. We also saw how the shell responded with the answer `15` when we added the numbers 5 and 10 together. 

In Python, this `5 + 10` line is called an expression. An expression is the most basic type of instructions you can write in a program. An expression typically consists of values (5 and 10) and operators (the addition operator "+"). Similar to mathematics, you can preform all basic arithmetic operations using Python expressions.

## Mathematical Operators in Python

| Type | Operator        | Expression     |
| ---- | --------------- | -------------- |
| `+`  | Addition        | `2 + 3 = 5`    |
| `-`  | Subtraction     | `8 - 1 = 7`    |
| `*`  | Multiplication  | `7 * 2 = 14`   |
| `/`  | Division        | `10 / 4 = 2.5` |
| `//` | Integer Divison | `10 / 4 = 2`   |
| `**` | Exponent        | `2**3 = 8`     |
| `%`  | Modulus         | `17 % 12 = 5`  |

## Order of Operations

Like in mathematics, the order of operators matter while evaluating an expression in Python. As a general rule, exponentiation is performed first, multiplication and division are performed next, addition and subtraction are performed last.

**Example:**

The expression `2 * 3 + 5` would evaluate to `11` as multiplication is evaluated before addition. `2 * 3` is evaluated first and results in `6`. `6` is then added to `5` which evaluates to `11`.

You can use parentheses to enforce a certain order. Expressions in parentheses evaluate before anything else.

**Example:**

`2 * (3 + 5)` would evalulate to `16`. The expression in parentheses is evaluated first and results in `8`. `8` is then multiplied by `2` which evaluates to `16`.

## Exercise

Open Python interactive shell on your computer and evaluate the following expressions. Can you write down the answer before executing the operations in the shell?

- `5 * 6 / 3 + 2`
- `2**4 * 2`
- `15 // 4 + 2`
- `100 / 10 + 5.5`
- `9 % 2 + 9 / 2`
