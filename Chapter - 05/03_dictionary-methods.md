# Dictionary Methods in Python

Dictionary methods are built-in functions used to perform various operations on dictionaries.

Consider the following dictionary:

```python
dic = {
    "Name": "Rahul",
    "From": "India",
    "Class": [10, 11, 12]
}
```

---

# 1. .items() Method

The `.items()` method returns all key-value pairs as tuples inside a special dictionary view object.

---

## Example

```python
print(dic.items())
```

---

## Output

```text
dict_items([
    ('Name', 'Rahul'),
    ('From', 'India'),
    ('Class', [10, 11, 12])
])
```

---

# 2. .keys() Method

The `.keys()` method returns all keys of the dictionary.

---

## Example

```python
print(dic.keys())
```

---

## Output

```text
dict_keys(['Name', 'From', 'Class'])
```

---

# 3. .values() Method

The `.values()` method returns all values of the dictionary.

---

## Example

```python
print(dic.values())
```

---

## Output

```text
dict_values(['Rahul', 'India', [10, 11, 12]])
```

---

# 4. .update() Method

The `.update()` method updates existing key-value pairs and can also add new key-value pairs.

---

## Example

```python
dic.update({
    "From": "Germany",
    "Subject": ["Phy", "Chem", "Maths"]
})

print(dic)
```

---

## Output

```text
{
    'Name': 'Rahul',
    'From': 'Germany',
    'Class': [10, 11, 12],
    'Subject': ['Phy', 'Chem', 'Maths']
}
```

### Explanation

- `"From"` is updated from `"India"` to `"Germany"`.
- `"Subject"` is added as a new key.

---

# 5. .get() Method

The `.get()` method returns the value of a specified key.

If the key does not exist, it returns a default value instead of producing an error.

---

## Example

```python
print(dic.get("Name", "Not Found"))
```

---

## Output

```text
Rahul
```

---

## Example with Missing Key

```python
print(dic.get("Age", "Not Found"))
```

---

## Output

```text
Not Found
```

---

# 6. .pop() Method

The `.pop()` method removes a specific key and returns its value.

---

## Example

```python
country = dic.pop("From")

print(country)
```

---

## Output

```text
India
```

---

### Dictionary After pop()

```python
{
    'Name': 'Rahul',
    'Class': [10, 11, 12]
}
```

---

# 7. .popitem() Method

The `.popitem()` method removes and returns the last inserted key-value pair as a tuple.

---

## Example

```python
last = dic.popitem()

print(last)
```

---

## Output

```text
('Class', [10, 11, 12])
```

---

# Summary Table

| Method | Purpose |
|----------|----------|
| `.items()` | Returns key-value pairs |
| `.keys()` | Returns all keys |
| `.values()` | Returns all values |
| `.update()` | Updates or adds key-value pairs |
| `.get()` | Returns value of a key |
| `.pop()` | Removes a specific key |
| `.popitem()` | Removes the last inserted key-value pair |

---

# Important Note

The difference between:

```python
dic["Name"]
```

and

```python
dic.get("Name")
```

is:

- `dic["Name"]` gives an error if the key does not exist.
- `dic.get("Name")` safely returns `None` (or a default value) if the key does not exist.