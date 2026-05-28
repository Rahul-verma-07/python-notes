# String Slicing in Python

String slicing is used to get a part of a string.

A string in Python can be sliced using indexes.

---

# String Indexing

Each character in a string has an index number.

## Example

```python
name = "Rahul"
```

```text
 R   A   H   U   L
 |   |   |   |   |
 0   1   2   3   4
 |   |   |   |   |
-5  -4  -3  -2  -1
```

---

# Important Note

- Positive indexing starts from `0`.
- Negative indexing starts from `-1`.
- The index of a string starts from:

```text
0 to (length - 1)
```

---

# Accessing Characters and String Slicing

## Example

```python
name = "Rahul"

name_short = name[0:3]

character_1 = name[0]
character_2 = name[-1]

print(name)

print(name_short)
# Sliced String

print(character_1)
# Single character from string

print(character_2)
# Single character from string

# Negative indices correspond to positive indices
print(name[-4:-1])

print(name[1:4])

print(name[:4])
# Same as name[0:4]

print(name[0:])
# Same as name[0:5]
```

---

# Output

```text
Rahul
Rah
R
l
ahu
ahu
Rahu
Rahul
```

---

# Explanation of Slicing

| Slice | Output | Meaning |
|---|---|---|
| `name[0:3]` | `Rah` | Index `0` to `2` |
| `name[1:4]` | `ahu` | Index `1` to `3` |
| `name[:4]` | `Rahu` | Starts from `0` automatically |
| `name[0:]` | `Rahul` | Goes till end automatically |
| `name[-4:-1]` | `ahu` | Negative index slicing |

---

# Slicing with Skip Value

Python also allows slicing with a skip value.

---

# Syntax

```python
string[start : end : skip]
```

Where:

- `start` → Starting index
- `end` → Ending limit
- `skip` → Number of indexes to skip

---

# Example

```python
num = "0123456789"

num_short = num[0:5]
# Simple slicing with positive indices

num_neg_short = num[-10:-1]
# Simple slicing with negative indices

num_skip_slice = num[0:5:2]
# Slicing with skip value

print(num)

print(num_short)

print(num_neg_short)

print(num_skip_slice)
```

---

# Output

```text
0123456789
01234
012345678
024
```

---

# Explanation of Skip Slicing

```python
num[0:5:2]
```

Means:

- Start from index `0`
- Go till index `4`
- Skip every `2` indexes

## Visualization

```text
0 1 2 3 4
↑   ↑   ↑

Output → 024
```

---

# Important Note

Strings in Python are immutable.

This means:

```text
Strings cannot be changed after creation.
```