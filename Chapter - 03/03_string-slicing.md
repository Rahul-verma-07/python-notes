# String Slicing in Python

String slicing is used to get a part of a string.

---

# Syntax

```python
string[start : end]
```

- `start` index is included.
- `end` index is excluded.

---

# Example

```python
name = "RAHUL"

print(name[0:3])
print(name[1:4])
print(name[:4])
print(name[2:])
```

---

# Output

```text
RAH
AHU
RAHU
HUL
```

---

# Explanation

| Slice | Output |
|---|---|
| `name[0:3]` | `RAH` |
| `name[1:4]` | `AHU` |
| `name[:4]` | `RAHU` |
| `name[2:]` | `HUL` |

---

# Negative Slicing Example

```python
name = "RAHUL"

print(name[-4:-1])
```

---

# Output

```text
AHU
```

---

# Important Note

- Strings in Python are immutable.

This means:

```text
Strings cannot be changed after creation.
```