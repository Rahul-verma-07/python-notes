# For Loop in Python

A `for` loop is used to iterate through a sequence such as:

- Lists
- Tuples
- Strings
- Sets
- Dictionaries

These objects are known as **iterables** because their elements can be accessed one by one.

---

# Syntax

```python
for variable in sequence:
    # Code to be executed
```

---

# How it Works

1. Python takes the first element from the sequence.
2. The element is assigned to the loop variable.
3. The loop body is executed.
4. Python moves to the next element.
5. This process continues until all elements have been processed.

---

# Example Using a List

```python
li = [1, 7, 8]

for item in li:
    print(item)
```

---

## Output

```text
1
7
8
```

---

# Example Using a Tuple

```python
tu = (10, 20, 30)

for item in tu:
    print(item)
```

---

## Output

```text
10
20
30
```

---

# Example Using a String

```python
name = "Rahul"

for character in name:
    print(character)
```

---

## Output

```text
R
a
h
u
l
```

---

# Flow of Execution

```text
      Sequence
          │
          ▼
   Take Next Element
          │
          ▼
   Execute Loop Body
          │
          ▼
 More Elements Left?
      │         │
     Yes       No
      │         │
      └────► Stop
```

---

# Real-Life Examples of For Loops

For loops are commonly used for:

- Traversing lists
- Processing strings
- Displaying menu items
- Reading data collections
- Pattern printing
- Repeating tasks a fixed number of times

---

# Important Note

> **NOTE:**
>
> - A `for` loop automatically moves through the sequence.
> - No manual increment (`i += 1`) is required.
> - The loop stops automatically after processing all elements.

---

# Comparison Between While Loop and For Loop

| While Loop | For Loop |
|------------|----------|
| Runs based on a condition | Runs over a sequence |
| Requires manual update of variable | Updates automatically |
| Useful when iterations are unknown | Useful when iterations are known |
| Can become infinite if not handled carefully | Stops automatically after sequence ends |