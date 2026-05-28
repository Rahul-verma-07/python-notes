# Tuple Methods in Python

Tuple methods and functions are used to perform operations on tuples.

Since tuples are immutable, most operations return new values instead of modifying the original tuple.

---

# Common Tuple Methods and Functions

1. `.count()`
2. `.index()`
3. `len()`
4. `max()`
5. `min()`
6. `sum()`
7. `sorted()`
8. `reversed()`

---

# 1. .count() Method

The `.count()` method returns the number of occurrences of a specific element in a tuple.

---

## Example

```python
a = (1, 2, 3, 4, 5)

count_of_3 = a.count(3)

print(count_of_3)
```

---

## Output

```text
1
```

---

# 2. .index() Method

The `.index()` method returns the index of the first occurrence of an element.

---

## Example

```python
a = (1, 2, 3, 4, 5)

index_of_3 = a.index(3)

print(index_of_3)
```

---

## Output

```text
2
```

---

# 3. len() Function

The `len()` function returns the total number of elements in a tuple.

---

## Example

```python
a = (1, 2, 3, 4, 5)

length_of_a = len(a)

print(length_of_a)
```

---

## Output

```text
5
```

---

# 4. max() Function

The `max()` function returns the largest element in a tuple.

---

## Example

```python
a = (1, 2, 3, 4, 5)

max_element = max(a)

print(max_element)
```

---

## Output

```text
5
```

---

# 5. min() Function

The `min()` function returns the smallest element in a tuple.

---

## Example

```python
a = (1, 2, 3, 4, 5)

min_element = min(a)

print(min_element)
```

---

## Output

```text
1
```

---

# 6. sum() Function

The `sum()` function returns the sum of all elements in a tuple.

---

## Example

```python
a = (1, 2, 3, 4, 5)

sum_of_elements = sum(a)

print(sum_of_elements)
```

---

## Output

```text
15
```

---

# 7. sorted() Function

The `sorted()` function returns a sorted list from the tuple elements.

> It does not modify the original tuple.

---

## Example

```python
a = (5, 4, 3, 2, 1)

sorted_a = sorted(a)

print(sorted_a)
```

---

## Output

```text
[1, 2, 3, 4, 5]
```

---

# Important Note

```python
sorted()
```

returns a list, not a tuple.

---

# 8. reversed() Function

The `reversed()` function returns a reversed iterator of the tuple elements.

---

## Example

```python
a = (1, 2, 3, 4, 5)

reversed_a = reversed(a)

print(list(reversed_a))
```

---

## Output

```text
[5, 4, 3, 2, 1]
```

---

# Important Notes

- Tuples are immutable.

This means:

```text
Tuple elements cannot be changed after creation.
```

- Functions like:

```python
sorted()
reversed()
```

do not modify the original tuple.

- They return new values instead.

---

# Difference Between Tuple Methods and Functions

| Method / Function | Purpose |
|---|---|
| `.count()` | Counts occurrences of an element |
| `.index()` | Returns index of an element |
| `len()` | Returns total number of elements |
| `max()` | Returns largest element |
| `min()` | Returns smallest element |
| `sum()` | Returns sum of elements |
| `sorted()` | Returns sorted list |
| `reversed()` | Returns reversed iterator |
 