# Tuples in Python

A tuple is an immutable data type in Python used to store multiple values.

Tuples can store values of different data types.

---

# Example of a Tuple

```python
tu = (7, 3.14, "RV")
```

```text
 Value →      7     3.14     "RV"
              |       |        |
Data Type → <int>  <float>   <str>
              |       |        |
Index →       0       1        2
              |       |        |
Neg Index →  -3      -2       -1
```

> Tuple indexing works exactly like lists and strings.

---

# Creating Tuples in Python

## Example

```python
# Empty Tuple
tu_01 = ()

print(tu_01)

# Tuple with one element
tu_02 = (1,)

print(tu_02)

# Tuple with multiple elements
tu_03 = (1, 2, 3, 4, 5)

print(tu_03)

print(type(tu_01))
print(type(tu_02))
print(type(tu_03))
```

---

# Output

```text
()
(1,)
(1, 2, 3, 4, 5)

<class 'tuple'>
<class 'tuple'>
<class 'tuple'>
```

---

# Important Note About Single Element Tuple

To create a tuple with only one element, a comma `,` is necessary.

## Correct Example

```python
tu = (1,)
```

---

## Incorrect Example

```python
tu = (1)
```

This is treated as:

```python
<class 'int'>
```

and not as a tuple.

---

# Accessing Tuple Elements

Tuple elements can be accessed using indexes.

## Example

```python
tu = (7, 3.14, "Rahul")

print(tu[0])
print(tu[1])
print(tu[2])
```

---

# Output

```text
7
3.14
Rahul
```

---

# Tuple Slicing

Tuples can also be sliced just like strings and lists.

## Example

```python
tu = (1, 2, 3, 4, 5)

print(tu[1:4])
```

---

## Output

```text
(2, 3, 4)
```

---

# Important Note

Tuples are immutable.

This means:

```text
Tuple elements cannot be changed after creation.
```

---

## Example

```python
tu = (1, 2, 3)

tu[0] = 10
```

---

## Error

```text
TypeError: 'tuple' object does not support item assignment
```

---

# Difference Between List and Tuple

| List | Tuple |
|---|---|
| Mutable | Immutable |
| Uses `[ ]` | Uses `( )` |
| Can be modified | Cannot be modified |