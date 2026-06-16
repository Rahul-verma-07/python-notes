# range() Function in Python

The `range()` function is used to generate a sequence of numbers.

It is commonly used with `for` loops to repeat a block of code a specific number of times.

---

# Syntax

```python
range(start, stop, step_size)
```

### Parameters

| Parameter | Description |
|------------|------------|
| `start` | Starting value of the sequence |
| `stop` | Ending value (not included) |
| `step_size` | Increment or decrement value |

---

# Important Note

- The `stop` value is **not included** in the sequence.
- The `step_size` parameter is optional.
- If `start` is not provided, Python assumes `0`.
- If `step_size` is not provided, Python assumes `1`.

---

# Example 1

```python
for i in range(0, 7):
    print(i)
```

---

## Output

```text
0
1
2
3
4
5
6
```

### Explanation

```python
range(0, 7)
```

starts from `0` and stops before `7`.

---

# Example 2

```python
for i in range(0, 7, 2):
    print(i)
```

---

## Output

```text
0
2
4
6
```

### Explanation

```python
range(0, 7, 2)
```

- Starts from `0`
- Stops before `7`
- Increases by `2` each time

---

# Example 3

```python
for i in range(5):
    print(i)
```

---

## Output

```text
0
1
2
3
4
```

### Explanation

When only one argument is provided:

```python
range(5)
```

Python assumes:

```python
range(0, 5)
```

---

# Example 4 (Reverse Counting)

```python
for i in range(10, 0, -1):
    print(i)
```

---

## Output

```text
10
9
8
7
6
5
4
3
2
1
```

### Explanation

The negative step value makes the sequence move backwards.

---

# For Loop with Else

An optional `else` block can be used with a `for` loop.

The `else` block executes when the loop completes normally without encountering a `break` statement.

---

# Syntax

```python
for variable in sequence:
    # Loop Body

else:
    # Executes after loop finishes
```

---

# Example

```python
li = [1, 7, 8]

for item in li:
    print(item)

else:
    print("Done")
```

---

## Output

```text
1
7
8
Done
```

### Explanation

After all elements of the list are processed, the `else` block is executed.

---

# Example with break

```python
for i in range(5):

    if i == 3:
        break

    print(i)

else:
    print("Done")
```

---

## Output

```text
0
1
2
```

### Explanation

The `else` block is **not executed** because the loop terminated using the `break` statement.

---

# Key Points

- `range()` generates a sequence of numbers.
- The `stop` value is never included.
- `step_size` controls the increment or decrement.
- `for-else` executes the `else` block only when the loop finishes normally.
- If a `break` statement is encountered, the `else` block is skipped.