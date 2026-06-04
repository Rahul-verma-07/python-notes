# String Indexing in Python

Each character in a string has a position number called an **index**.

Python supports two types of indexing:

1. Positive Indexing
2. Negative Indexing

---

# Example String

```python
name = "RAHUL"
```

---

# Positive Indexing

Positive indexing starts from `0` and moves from left to right.

```text
 R   A   H   U   L
 |   |   |   |   |
 0   1   2   3   4
```

---

# Negative Indexing

Negative indexing starts from `-1` and moves from right to left.

```text
 R   A   H   U   L
 |   |   |   |   |
-5  -4  -3  -2  -1
```

---

# Accessing Characters Using Indexing

## Example

```python
name = "RAHUL"

print(name[0])
print(name[1])
print(name[2])
print(name[-2])
print(name[-1])
```

---

# Output

```text
R
A
H
U
L
```