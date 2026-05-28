# Lists in Python

A list in Python is a container used to store multiple values of different data types.

Lists are ordered and indexed.

---

# Example of a List

```python
li = [7, 3.14, "RV"]
```

```text
 Value →     7      3.14      "RV"
              |        |         |
Data Type → <int>   <float>   <str>
              |        |         |
Index →       0        1         2
              |        |         |
Neg Index →  -3       -2        -1
```

---

# Creating a List

## Example

```python
li = [7, 3.14, "Rahul", True, None]

print(li)
print(type(li))
```

---

# Output

```text
[7, 3.14, 'Rahul', True, None]
<class 'list'>
```

---

# Accessing Elements of a List

List elements can be accessed using indexes.

## Example

```python
li = [7, 3.14, "Rahul", True, None]

print(li[0])
# First element

print(li[1])
# Second element

print(li[2])
# Third element

print(li[3])
# Fourth element

print(li[4])
# Fifth element
```

---

# Output

```text
7
3.14
Rahul
True
None
```

---

# Index Error

Accessing an index that does not exist produces an error.

## Example

```python
print(li[5])
```

---

## Error

```text
IndexError: list index out of range
```

---

# List Slicing

Lists can be sliced just like strings.

---

## Syntax

```python
list[start : end]
```

- `start` index is included
- `end` index is excluded

---

## Example

```python
li = [7, 3.14, "Rahul", True, None]

print(li[0:3])
```

---

## Output

```text
[7, 3.14, 'Rahul']
```

---

# Negative Indexing in Lists

Python also supports negative indexing in lists.

## Example

```python
li = [7, 3.14, "Rahul"]

print(li[-1])
print(li[-2])
print(li[-3])
```

---

## Output

```text
Rahul
3.14
7
```

---

# Important Note

Lists in Python are mutable.

This means:

```text
List elements can be changed after creation.
```

---

# Example of Mutable List

```python
li = [7, 3.14, "Hello"]

print(li[2])

li[2] = "Python"

print(li[2])
```

---

# Output

```text
Hello
Python
```

---

# Explanation

In the above example:

```python
li[2] = "Python"
```

changes the value at index `2`.

Unlike strings, lists can be modified easily.