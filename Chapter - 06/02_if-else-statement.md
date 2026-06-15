# if-else Statement in Python

The `if-else` statement is used to make decisions in a program.

It allows Python to execute different blocks of code depending on whether a condition is `True` or `False`.

---

# Syntax

```python
if condition:
    # Code executed when condition is True
    print("DONE")
else:
    # Code executed when condition is False
    print("INCOMPLETE")
```

---

# How it Works

1. Python checks the condition inside the `if` statement.
2. If the condition is `True`, the code inside the `if` block is executed.
3. If the condition is `False`, the code inside the `else` block is executed.

---

# Example 1

```python
age = 18

if age >= 18:
    print("Eligible to Vote")
else:
    print("Not Eligible to Vote")
```

---

## Output

```text
Eligible to Vote
```

---

# Example 2

```python
marks = 35

if marks >= 40:
    print("Passed")
else:
    print("Failed")
```

---

## Output

```text
Failed
```

---

# Flow of Execution

```text
        Condition
            │
      ┌─────┴─────┐
      │           │
    True       False
      │           │
 Execute      Execute
 if Block    else Block
```

---

# Real-Life Examples

The `if-else` statement is commonly used for:

- Checking voting eligibility
- Login authentication
- Pass or fail decisions
- ATM transactions
- Age verification
- Game logic

---

# Important Note

Only one block is executed at a time:

- If the condition is `True`, the `if` block runs.
- If the condition is `False`, the `else` block runs.