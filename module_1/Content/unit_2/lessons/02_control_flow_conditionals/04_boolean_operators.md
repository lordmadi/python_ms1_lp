Boolean operators are used to compare Boolean values (`True` and `False`). Like comparison operators, they evaluate expressions and return `True` or `False`, based on a specific condition or a set of conditions.

## Logic & Programming

Programmers work with logic quite a lot when building programs. As humans, statements that we use in real life must "make sense" for us to comprehend and process. 

In the previous concept, we evaluated comparisons using comparison operators and logic behind the scenes. `5 > 2` evaluates to `True` because logically it's true. 

In addition to that, we can use logic to evaluate some statements based on a certain context. Let's observe some examples.

## The `and` Operator

You're on a summer vacation and you'd like to go swimming in the sea. You want to only swim in the sea if the waves are not strong **and** if the water is considerably warm. The conditions you set can be rephrased as follows:

- If the sea water is warm **and** the waves aren't strong, I'll go swimming.

In this example, failing either of the two conditions (warm water and weak waves) will prevent you from swimming. In this context, we can say that a conjuction of two conditions with the `and` keyword dictates that both of them must be `True` in order for the entire statement to be `True`. If any of them is `False`, the whole statement evaluates to `False.`

## The `or` Operator

You head to a restaurant to grab dinner. You only eat chicken or sea food. If either of them is on the menu, you will make an order. Otherwise, you'll look for another restaurant. The conditions you set can be rephrased as follows:

- If I find chicken **or** sea food on the menu, I'll make an order.

In this example, failing either of the two conditions (finding chicken or finding sea food) will not prevent you from making an order. Only failing **both** of them will do so. In this context, we can say that a conjuction of two conditions with the `or` keyword dictates that either of them must be `True` in order for the entire statement to be `True`. If both of them are `False`, the whole statement evaluates to `False.`

## The `not` operator

This operator negates a condition. It acts as a flip switch that converts `True` to `False` and `False` to `True`.

Based on these examples, we can determine the evaluation results on statements that use `and` and `or` conjunctions in the following truth table:

| Expression        | Evaluation |
| ----------------- | ---------- |
| `True and True`   | True       |
| `True and False`  | False      |
| `False and True`  | False      |
| `False and False` | False      |
| `True or True`    | True       |
| `True or False`   | True       |
| `False or True`   | True       |
| `True or False`   | False      |
| `not True`        | False      |
| `not False`       | True       |


## Mixing Comparison & Boolean Operators

Armed with the knowledge we obtained in the previous concept and this concept, we can write more complex statements that combine both comparison and boolean operators.

```python
print((4 > 3) and (2 < 2)) # False
print("hello" == "hello" and (5 == 5)) # True
print((3 != 3) or (10 > 10)) # False
print((17.5 >= 17)) or (19 > 35) # True
print((7 == 7) and (not False)) # True
```

> When the first condition in an **or** statement evaluates to true, you can skip evaluating the rest of the conditions. This is known as "short-circuiting".

We can also combine more than 2 conditions in the same statement.

```python
print((5 > 3) and (2 > 1) and (3 > 2) or (1 < 0.5)) # True
```

In this example, we evaluated `5 > 3 and 2 > 1` first, the result is `True`. We then evaluated `3 > 2 or 1 < 0.5`, the result is `True`. Then, evaluating both results with the `and` operator as a conjunction gives us `True`.

It's important to keep in mind that boolean operators have an order of operations like mathematical operators. Math and comparison operations are evaulated first, then Python evaluates `not`, followed by `and`, and then `or`.

## Exercise

Evaluate the following expressions and state whether they are `True` or `False`.

- `"hello" == "Hello" and 5 == 5`
- `5 > 2 and 3.5 < 3`
- `True and False and False or True`
- `(True and False) and (False or True)`
- `10 == "10" and not True or 2 < 10`
- `15.5 <= 15.55 and 31 == "thirty-one" and not False`