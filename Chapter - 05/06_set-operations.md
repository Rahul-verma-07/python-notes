# Operations on Sets in Python

Sets provide various built-in methods and operations to manipulate data efficiently.

Consider the following empty set:

```python
s = set()

print(s, type(s))
```

---

## Output

```text
set() <class 'set'>
```

---

# 1. len() Function

The `len()` function returns the total number of elements in a set.

## Example

```python
s = set()

print(len(s))
```

---

## Output

```text
0
```

---

# 2. .add() Method

The `.add()` method adds an element to a set.

## Example

```python
s = set()

s.add(1)
s.add(2)

print(s)
```

---

## Output

```text
{1, 2}
```

---

# 3. .remove() Method

The `.remove()` method removes a specified element from a set.

## Example

```python
s = {1, 2}

s.remove(1)

print(s)
```

---

## Output

```text
{2}
```

> If the element does not exist, Python raises a `KeyError`.

---

# 4. .pop() Method

The `.pop()` method removes and returns an arbitrary element from the set.

## Example

```python
s = {1, 2}

print(s.pop())
print(s)
```

---

## Possible Output

```text
1
{2}
```

> Since sets are unordered, the removed element may vary.

---

# 5. .clear() Method

The `.clear()` method removes all elements from the set.

## Example

```python
s = {1, 2}

s.clear()

print(s)
```

---

## Output

```text
set()
```

---

# 6. .union() Method

The `.union()` method returns a new set containing all unique elements from both sets.

## Example

```python
s = {1, 2, 3, 4, 5}

s2 = {3, 4, 5, 6, 7}

print(s.union(s2))
```

---

## Output

```text
{1, 2, 3, 4, 5, 6, 7}
```

---

# 7. .intersection() Method

The `.intersection()` method returns a new set containing only the common elements.

## Example

```python
s = {1, 2, 3, 4, 5}

s2 = {3, 4, 5, 6, 7}

print(s.intersection(s2))
```

---

## Output

```text
{3, 4, 5}
```

---

# Additional Set Operations

## Example

```python
r1 = {1, 2, 3}
r3 = {3, 4, 5}

r2 = r1.intersection(r3)

print(r2)

print(r1.union(r2.union(r3)))

print(r1.difference(r3))
print(r3.difference(r1))

print(r1.symmetric_difference(r3))

print(r1.issubset(r3))
print(r1.issuperset(r3))
```

---

## Output

```text
{3}

{1, 2, 3, 4, 5}

{1, 2}

{4, 5}

{1, 2, 4, 5}

False

False
```

---

# 8. .difference() Method

Returns elements that exist in the first set but not in the second set.

## Example

```python
r1 = {1, 2, 3}
r3 = {3, 4, 5}

print(r1.difference(r3))
```

---

## Output

```text
{1, 2}
```

---

# 9. .symmetric_difference() Method

Returns elements that are present in either set, but not in both.

## Example

```python
r1 = {1, 2, 3}
r3 = {3, 4, 5}

print(r1.symmetric_difference(r3))
```

---

## Output

```text
{1, 2, 4, 5}
```

---

# 10. .issubset() Method

Checks whether all elements of one set are present in another set.

## Example

```python
r1 = {1, 2}
r2 = {1, 2, 3, 4}

print(r1.issubset(r2))
```

---

## Output

```text
True
```

---

# 11. .issuperset() Method

Checks whether a set contains all elements of another set.

## Example

```python
r2 = {1, 2, 3, 4}
r1 = {1, 2}

print(r2.issuperset(r1))
```

---

## Output

```text
True
```

---

# Summary Table

| Method | Purpose |
|----------|----------|
| `len()` | Returns number of elements |
| `.add()` | Adds an element |
| `.remove()` | Removes an element |
| `.pop()` | Removes a random element |
| `.clear()` | Removes all elements |
| `.union()` | Combines two sets |
| `.intersection()` | Returns common elements |
| `.difference()` | Returns unique elements of first set |
| `.symmetric_difference()` | Returns non-common elements |
| `.issubset()` | Checks subset relation |
| `.issuperset()` | Checks superset relation |

---

# Important Note

Sets are extremely useful when:

- Duplicate values must be removed.
- Fast membership testing is required.
- Mathematical set operations are needed.
