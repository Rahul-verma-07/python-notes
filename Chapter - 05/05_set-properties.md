# Properties of Sets in Python

Sets have several important properties that distinguish them from other data types such as lists, tuples, and dictionaries.

---

# 1. Sets are Unordered

The order of elements in a set does not matter.

Python may display set elements in a different order each time.

## Example

```python
s = {10, 20, 30, 40}

print(s)
```

---

## Possible Output

```text
{40, 10, 20, 30}
```

> The order may vary depending on the Python interpreter.

---

# 2. Sets are Unindexed

Sets do not support indexing.

This means elements cannot be accessed using index numbers.

## Example

```python
s = {10, 20, 30}

print(s[0])
```

---

## Error

```text
TypeError: 'set' object is not subscriptable
```

---

# 3. Set Elements Cannot Be Changed Directly

Individual elements of a set cannot be modified using indexes because sets are unindexed.

## Invalid Example

```python
s = {10, 20, 30}

s[0] = 100
```

---

## Error

```text
TypeError
```

### However

You can:

- Add elements using `.add()`
- Remove elements using `.remove()`

---

## Example

```python
s = {10, 20, 30}

s.add(40)

print(s)
```

---

## Output

```text
{10, 20, 30, 40}
```

---

# 4. Sets Cannot Contain Duplicate Values

A set stores only unique elements.

Duplicate values are automatically removed.

## Example

```python
s = {1, 2, 2, 3, 3, 4, 4}

print(s)
```

---

## Output

```text
{1, 2, 3, 4}
```

### Explanation

Even though some values appear multiple times, the set keeps only one copy of each value.

---

# Summary

| Property | Description |
|-----------|-------------|
| Unordered | Element order does not matter |
| Unindexed | Elements cannot be accessed using indexes |
| Mutable | Elements can be added or removed |
| No Duplicates | Duplicate values are automatically removed |

---

# Important Note

Sets are useful when:

- You need unique values.
- Duplicate data should be removed automatically.
- Element order is not important.