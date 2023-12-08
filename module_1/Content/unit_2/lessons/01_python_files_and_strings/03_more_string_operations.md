In the previous concept, we knew for a fact that we can't modify strings after they are created. That being said, we can still benefit from accessing the characters of a string by its index. 

## String Slicing

In Python, we can access a portion of a string by specifying start and end indices. The start index specifies where the slicing begins and the end index specifies where it should stop. It's important to know that the end index is **not included** in the sliced portion.

```python
item_description = "Red Car"
color = item_description[0:3] 
print(color) # Red
```

> Notice that we set the end index to be `3` since we want the whole word `Red` to be included in the sliced portion.

You can ignore the start index if you are going to slice from the beginning of the string.

```python
item_description = "Red Car"
color = item_description[:3] 
print(color) # Red
```
Similarly, you can also ignore the end index if you are going to slice up to the end of the string.

```python
item_description = "Red Car"
color = item_description[4:] 
print(color) # Car
```

## Exercise

**Access the following strings using correct indices to obtain the required substrings.**

| String          | Substring to Extract |
| --------------- | -------------------- |
| January         | ary                  |
| Banana          | Ba                   |
| Mount Fuji      | Fuji                 |
| Carbon Dioxide  | oxide                |
| Spider Man      | Spi                  |
| JavaScript      | Java                 |
| 6th of December | 6th of Dec           |

**Slice the bold parts from strings one and two  and concatenate them together. Save the result in a new variable.

| String One        | String Two        | Wanted Result |
| ----------------- | ----------------- | ------------- |
| **Milk** Tea      | Protein **Shake** | Milk Shake    |
| **Barren** Fields | High **Summit**   | Barren Summit |
| **Val**kyrie      | C**halla**h Bread | Valhalla      |


