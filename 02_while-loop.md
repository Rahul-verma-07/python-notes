# While Loop in Python

A `while` loop is used to repeatedly execute a block of code as long as a given condition remains `True`.

Before each iteration, Python checks the condition.

- If the condition is `True`, the loop body is executed.
- If the condition is `False`, the loop stops.

---

# Syntax

```python
while condition:
    # Body of the loop
```

---

# How it Works

1. Python checks the condition.
2. If the condition is `True`, the loop body executes.
3. After execution, Python checks the condition again.
4. This process continues until the condition becomes `False`.

---

# Example

```python
i = 1

while i <= 5:
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
      Condition
          │
     ┌────┴────┐
     │         │
   True      False
     │         │
 Execute     Stop
 Loop Body   Loop
     │
     └─────────► Check Condition Again
```

---

# Example: Printing Numbers from 1 to 10

```python
i = 1

while i <= 10:
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
6
7
8
9
10
```

---

# Important Note

> **NOTE:**
>
> - If the condition never becomes `False`, the loop continues forever.
> - Such a loop is called an **Infinite Loop**.

---

# Infinite Loop Example

```python
while True:
    print("Hello")
```

### Output

```text
Hello
Hello
Hello
...
```

The loop never stops because the condition:

```python
True
```

always remains `True`.

---

# Real-Life Examples of While Loops

While loops are commonly used for:

- Taking user input repeatedly
- Password validation
- Menu-driven programs
- Game loops
- Repeating tasks until a condition is met

---

# Key Points

- `while` loops execute as long as the condition is `True`.
- The condition is checked before every iteration.
- If the condition is initially `False`, the loop body will not execute even once.
- Always ensure that the condition eventually becomes `False` to avoid infinite loops.