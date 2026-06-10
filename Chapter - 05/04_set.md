# Sets in Python

A set is a collection of unique (non-repetitive) elements.

Sets automatically remove duplicate values and store only distinct elements.

---

# Syntax

## Empty Set

```python
s = set()
```

> An empty set cannot be created using `{}` because `{}` creates an empty dictionary.

---

## Creating a Set

```python
s = {1, 2, 3}
```

---

# Example

```python
s = set()

s.add(2)
s.add(1)

print(s)
```

---

## Output

```text
{1, 2}
```

---

# Another Example

```python
s = {1, 42, 22}

print(s)
```

---

## Output

```text
{1, 42, 22}
```

---

# Duplicate Values in a Set

Sets do not allow duplicate values.

## Example

```python
s = {1, 2, 2, 3, 3, 3, 4}

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

# Adding Elements to a Set

The `.add()` method is used to add elements to a set.

## Example

```python
s = set()

s.add(10)
s.add(20)

print(s)
```

---

## Output

```text
{10, 20}
```

---

# Important Properties of Sets

- Sets store only unique values.
- Sets are unordered.
- Sets are mutable.
- Sets do not support indexing.
- Duplicate values are automatically removed.

---

# Important Note

Unlike lists, tuples, and strings:

```python
s = {1, 2, 3}
```

This is invalid:

```python
print(s[0])
```

because sets do not support indexing.

---

## Error

```text
TypeError: 'set' object is not subscriptable
```