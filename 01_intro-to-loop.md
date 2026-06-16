# Loops in Python

Sometimes we need to execute a set of statements repeatedly.

For example, printing numbers from `1` to `1000` manually would be time-consuming and inefficient.

Loops allow a programmer to execute the same block of code multiple times without writing it again and again.

---

# Why Use Loops?

Without loops:

```python
print(1)
print(2)
print(3)
print(4)
print(5)
```

With loops:

```python
for i in range(1, 6):
    print(i)
```

Both produce the same output, but loops make the code shorter, cleaner, and easier to maintain.

---

# Types of Loops in Python

Python provides two main types of loops:

1. `while` Loop
2. `for` Loop
---

# Important Note

Loops help reduce code duplication and make programs more efficient.

A loop continues to execute until:

- The condition becomes `False` (`while` loop), or
- All items in the sequence are processed (`for` loop).