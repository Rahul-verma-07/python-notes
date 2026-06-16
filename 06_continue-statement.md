# Continue Statement in Python

The `continue` statement is used to skip the current iteration of a loop and move directly to the next iteration.

When Python encounters a `continue` statement, it ignores the remaining code inside the loop for that iteration and starts the next iteration immediately.

---

# Why Use continue?

Sometimes we want to skip specific values or conditions while keeping the loop running.

The `continue` statement allows us to do this.

---

# Syntax

```python
for variable in sequence:

    if condition:
        continue

    # Loop Body
```

---

# Example

```python
for i in range(0, 8):

    if i == 5:
        continue

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
6
7
```

### Explanation

When the value of `i` becomes `5`:

```python
if i == 5:
    continue
```

Python skips that iteration and moves directly to the next value.

Therefore, `5` is not printed.

---

# Example with while Loop

```python
i = 0

while i < 8:

    i += 1

    if i == 5:
        continue

    print(i)
```

---

## Output

```text
1
2
3
4
6
7
8
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
 Execute      Execute
 Remaining    continue
 Code            │
     │            │
     └────────────┘
            │
            ▼
      Next Iteration
```

---

# Example: Skip Even Numbers

```python
for i in range(1, 11):

    if i % 2 == 0:
        continue

    print(i)
```

---

## Output

```text
1
3
5
7
9
```

### Explanation

Whenever an even number is encountered, Python skips that iteration.

---

# Real-Life Examples

The `continue` statement is commonly used for:

- Filtering data
- Skipping invalid input
- Ignoring unwanted values
- Processing selected records
- Game development logic

---

# Important Note

> **NOTE:**
>
> - `continue` does not terminate the loop.
> - It only skips the current iteration.
> - The loop continues normally with the next iteration.

---

# Difference Between break and continue

| break | continue |
|---------|---------|
| Terminates the loop completely | Skips only the current iteration |
| Loop stops immediately | Loop continues running |
| Control moves outside the loop | Control moves to the next iteration |

---

# Example Comparison

```python
# break

for i in range(5):

    if i == 3:
        break

    print(i)
```

### Output

```text
0
1
2
```

---

```python
# continue

for i in range(5):

    if i == 3:
        continue

    print(i)
```

### Output

```text
0
1
2
4
```