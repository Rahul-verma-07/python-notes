# Properties of Dictionaries in Python

Python dictionaries have some important properties that make them useful for storing and managing data.

---

# 1. Dictionaries are Unordered

Dictionaries store data as key-value pairs.

Traditionally, elements are not accessed using index positions like lists or tuples.

Instead, values are accessed using their keys.

## Example

```python
student = {
    "Name": "Rahul",
    "Marks": 95
}

print(student["Name"])
```

---

## Output

```text
Rahul
```

---

# 2. Dictionaries are Mutable

Dictionaries can be modified after creation.

This means:

- Values can be changed
- New key-value pairs can be added
- Existing key-value pairs can be removed

## Example

```python
student = {
    "Name": "Rahul",
    "Marks": 95
}

student["Marks"] = 100

print(student)
```

---

## Output

```text
{'Name': 'Rahul', 'Marks': 100}
```

---

# 3. Dictionaries are Indexed Using Keys

Unlike lists and tuples, dictionaries are accessed using keys instead of numerical indexes.

## Example

```python
student = {
    "Name": "Rahul",
    "Marks": 95
}

print(student["Marks"])
```

---

## Output

```text
95
```

---

# 4. Duplicate Keys are Not Allowed

A dictionary cannot contain duplicate keys.

If the same key is written multiple times, the last value overwrites the previous value.

## Example

```python
student = {
    "Name": "Rahul",
    "Name": "Shlok"
}

print(student)
```

---

## Output

```text
{'Name': 'Shlok'}
```

### Explanation

The key:

```python
"Name"
```

appears twice.

Python keeps only the last value associated with that key.

---

# Summary

| Property | Description |
|-----------|-------------|
| Unordered | Data is stored as key-value pairs |
| Mutable | Values can be changed after creation |
| Indexed by Keys | Access values using keys |
| No Duplicate Keys | Duplicate keys are automatically overwritten |

---

# Important Note

Dictionary keys must be unique, but values can be duplicated.

## Example

```python
student = {
    "Rahul": 90,
    "Shlok": 90
}
```

This is perfectly valid because:

- Keys are different
- Values can be the same