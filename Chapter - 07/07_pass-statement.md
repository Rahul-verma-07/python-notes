# Pass Statement in Python

The `pass` statement is a null statement in Python.

It instructs Python to do nothing when it is executed.

The `pass` statement is often used as a placeholder when a statement is required syntactically, but no code needs to be written yet.

---

# Why Use pass?

Sometimes a block of code is required, but we have not decided what to write inside it.

In such cases, we can use the `pass` statement to avoid syntax errors.

---

# Syntax

```python
pass
```

---

# Example with Loop

```python
li = [1, 7, 8]

for i in li:
    pass
```

---

## Output

```text
No Output
```

### Explanation

The loop iterates through all elements of the list, but:

```python
pass
```

does nothing, so nothing is printed.

---

# Example Without pass

```python
li = [1, 7, 8]

for i in li:
```

---

## Error

```text
IndentationError: expected an indented block
```

### Explanation

Python expects a statement inside the loop body.

Using `pass` provides an empty statement and prevents this error.

---

# Example with if Statement

```python
age = 18

if age >= 18:
    pass

print("Program Executed Successfully")
```

---

## Output

```text
Program Executed Successfully
```

---

# Example with Function

```python
def greet():
    pass
```

This creates an empty function that can be completed later.

---

# Real-Life Uses of pass

The `pass` statement is commonly used for:

- Creating placeholder functions
- Creating placeholder classes
- Writing incomplete programs
- Testing program structure
- Avoiding syntax errors during development

---

# Difference Between pass and continue

| pass | continue |
|--------|--------|
| Does nothing | Skips current iteration |
| Used as a placeholder | Used inside loops |
| Program continues normally | Moves to next iteration |
| Can be used anywhere | Only meaningful inside loops |

---

# Example Comparison

```python
# pass

for i in range(5):

    if i == 2:
        pass

    print(i)
```

### Output

```text
0
1
2
3
4
```

---

```python
# continue

for i in range(5):

    if i == 2:
        continue

    print(i)
```

### Output

```text
0
1
3
4
```

---

# Important Note

> **NOTE:**
>
> - `pass` does not stop a loop.
> - `pass` does not skip an iteration.
> - `pass` simply acts as a placeholder and performs no action.
> - It is useful when Python requires a statement but no code is needed yet.