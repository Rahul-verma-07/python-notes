# Break Statement in Python

The `break` statement is used to immediately terminate a loop.

When Python encounters a `break` statement, it exits the loop instantly and continues execution with the first statement after the loop.

---

# Why Use break?

Sometimes we want to stop a loop before it finishes all iterations.

The `break` statement allows us to do this.

---

# Syntax

```python
for variable in sequence:

    if condition:
        break

    # Loop Body
```

---

# Example

```python
for i in range(0, 8):

    if i == 5:
        break

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

When the value of `i` becomes `5`:

```python
if i == 5:
    break
```

the loop stops immediately.

Therefore, numbers after `4` are never printed.

---

# Example with while Loop

```python
i = 1

while i <= 10:

    if i == 6:
        break

    print(i)

    i += 1
```

---

## Output

```text
1
2
3
4
5
```

---

# Flow of Execution

```text
      Loop Running
            │
            ▼
     Check Condition
            │
     ┌──────┴──────┐
     │             │
  False          True
     │             │
 Continue      Execute
 Loop          break
     │             │
     └──────► Exit Loop
```

---

# Real-Life Examples

The `break` statement is commonly used for:

- Menu-driven programs
- Password validation
- Search operations
- Finding a specific element
- Game controls
- Stopping infinite loops

---

# Example: Search an Element

```python
numbers = [2, 5, 8, 10, 15]

for num in numbers:

    if num == 10:
        print("Found")
        break
```

---

## Output

```text
Found
```

### Explanation

As soon as `10` is found, the loop stops.

---

# Important Note

> **NOTE:**
>
> - `break` immediately exits the nearest loop.
> - Statements after `break` inside the loop are not executed.
> - If a `for-else` loop contains a `break`, the `else` block is skipped.

---

# Example with for-else

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

The `else` block is not executed because the loop ended using `break`.