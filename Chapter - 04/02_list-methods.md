# List Methods in Python

List methods are built-in functions used to perform operations on lists.

---

# Common List Methods

1. `.sort()`
2. `.append()`
3. `.reverse()`
4. `.insert()`
5. `.remove()`
6. `.pop()`
7. `.index()`
8. `.count()`
9. `.extend()`
10. `sum()`

---

# 1. .sort() Method

The `.sort()` method sorts the list in ascending order.

---

## Example

```python
li = [2, 3, 1, 4]

print(li)

li.sort()

print(li)
```

---

## Output

```text
[2, 3, 1, 4]
[1, 2, 3, 4]
```

---

# 2. .append() Method

The `.append()` method adds an element at the end of the list.

---

## Example

```python
li = [2, 3, 1, 4]

print(li)

li.append(5)

print(li)
```

---

## Output

```text
[2, 3, 1, 4]
[2, 3, 1, 4, 5]
```

---

# 3. .reverse() Method

The `.reverse()` method reverses the order of list elements.

---

## Example

```python
li = [2, 3, 1, 4]

print(li)

li.reverse()

print(li)
```

---

## Output

```text
[2, 3, 1, 4]
[4, 1, 3, 2]
```

---

# 4. .insert() Method

The `.insert()` method inserts an element at a specific index.

---

## Example

```python
li = [2, 3, 1, 4]

print(li)

li.insert(2, 6)

print(li)
```

---

## Output

```text
[2, 3, 1, 4]
[2, 3, 6, 1, 4]
```

### Explanation

```python
li.insert(2, 6)
```

means:

- Insert `6`
- At index `2`

---

# 5. .remove() Method

The `.remove()` method removes the first occurrence of a specific element.

---

## Example

```python
li = [2, 3, 1, 4, 6]

print(li)

li.remove(6)

print(li)
```

---

## Output

```text
[2, 3, 1, 4, 6]
[2, 3, 1, 4]
```

---

# 6. .pop() Method

The `.pop()` method removes and returns the element at a specific index.

---

## Example

```python
li = [2, 3, 1, 4]

print(li)

last_element = li.pop(3)

print(li)

print(last_element)
```

---

## Output

```text
[2, 3, 1, 4]
[2, 3, 1]
4
```

---

# 7. .index() Method

The `.index()` method returns the index of the first occurrence of an element.

---

## Example

```python
li = [2, 3, 1, 4]

print(li)

index_of_4 = li.index(4)

print(index_of_4)
```

---

## Output

```text
[2, 3, 1, 4]
3
```

---

# 8. .count() Method

The `.count()` method returns the number of occurrences of an element.

---

## Example

```python
li = [2, 3, 1, 4]

print(li)

count_of_4 = li.count(4)

print(count_of_4)
```

---

## Output

```text
[2, 3, 1, 4]
1
```

---

# 9. .extend() Method

The `.extend()` method adds elements from another iterable or list.

---

## Example

```python
li = [2, 3, 1, 4]

li_2 = [5, 6, 7]

print(li)

li.extend(li_2)

print(li)
```

---

## Output

```text
[2, 3, 1, 4]
[2, 3, 1, 4, 5, 6, 7]
```

---

# 10. sum() Function

The `sum()` function returns the total sum of all elements in a list.

---

## Example

```python
li = [2, 3, 1, 4]

print(li)

total = sum(li)

print(total)
```

---

## Output

```text
[2, 3, 1, 4]
10
```

---

# Important Note

- List methods directly modify the original list.
- Lists in Python are mutable.

This means:

```text
Lists can be changed after creation.
```