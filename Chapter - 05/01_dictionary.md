# Dictionaries in Python

A dictionary is a collection of **key-value pairs**.

Dictionaries are used to store data in a structured way, where each value is associated with a unique key.

---

# Syntax

```python
dictionary_name = {
    "key1": value1,
    "key2": value2,
    "key3": value3
}
```

---

# Example

```python
dic = {
    "Name": "Rahul",
    "Class": [80, 90, 100],
    "Rahul": 80,
    "Shlok": 90,
    "Total": 100
}

print(dic["Name"])
print(dic["Rahul"])
print(dic["Shlok"])
print(dic["Total"])
```

---

# Output

```text
Rahul
80
90
100
```

---

# Understanding Key-Value Pairs

```python
dic = {
    "Name": "Rahul"
}
```

Here:

| Key | Value |
|------|------|
| `"Name"` | `"Rahul"` |

The key is used to access its corresponding value.

---

# Accessing Values

Values in a dictionary are accessed using their keys.

## Example

```python
dic = {
    "Name": "Rahul",
    "Age": 18
}

print(dic["Name"])
print(dic["Age"])
```

---

## Output

```text
Rahul
18
```

---

# Dictionary Can Store Different Data Types

A dictionary can store:

- Integers
- Floats
- Strings
- Lists
- Tuples
- Booleans
- Other Dictionaries

## Example

```python
student = {
    "Name": "Rahul",
    "Age": 18,
    "Marks": [80, 90, 100],
    "Passed": True
}

print(student)
```

---

# Important Features of Dictionaries

- Dictionaries store data as **key-value pairs**.
- Keys must be unique.
- Values can be duplicated.
- Dictionaries are mutable.
- Dictionaries are enclosed within `{ }` braces.

---

# Important Note

Unlike lists and tuples, dictionaries are not accessed using indexes.

Instead, they are accessed using keys.

### List

```python
li = [10, 20, 30]

print(li[0])
```

### Dictionary

```python
dic = {
    "Marks": 100
}

print(dic["Marks"])
```