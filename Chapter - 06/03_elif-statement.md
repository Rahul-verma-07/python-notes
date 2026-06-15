# if-elif-else Statement in Python

The `if-elif-else` statement is used when a program needs to check multiple conditions.

Python evaluates the conditions one by one and executes the block corresponding to the first condition that is `True`.

If none of the conditions are `True`, the `else` block is executed.

---

# Syntax

```python
if condition1:
    print("DONE")

elif condition2:
    print("MAY BE")

else:
    print("INCOMPLETE")
```

---

# How it Works

1. Python checks `condition1`.
2. If `condition1` is `True`, the `if` block executes.
3. Otherwise, Python checks `condition2`.
4. If `condition2` is `True`, the `elif` block executes.
5. If none of the conditions are `True`, the `else` block executes.

---

# Example 1

```python
marks = 85

if marks >= 90:
    print("Grade A+")

elif marks >= 75:
    print("Grade A")

else:
    print("Grade B")
```

---

## Output

```text
Grade A
```

---

# Example 2

```python
age = 17

if age >= 18:
    print("Eligible to Vote")

elif age >= 16:
    print("Can Apply Soon")

else:
    print("Not Eligible")
```

---

## Output

```text
Can Apply Soon
```

---

# Flow of Execution

```text
          Condition 1
               │
        ┌──────┴──────┐
        │             │
      True          False
        │             │
   Execute IF     Condition 2
                      │
               ┌──────┴──────┐
               │             │
             True          False
               │             │
        Execute ELIF    Execute ELSE
```

---

# Real-Life Examples

The `if-elif-else` statement is commonly used for:

- Grading systems
- Traffic light systems
- ATM menu options
- Login systems
- Weather applications
- Age-based classifications

---

# Important Note

- Multiple `elif` statements can be used.
- Only one block is executed.
- Once a condition becomes `True`, Python skips all remaining conditions.

---

# Example with Multiple elif

```python
marks = 72

if marks >= 90:
    print("Grade A+")

elif marks >= 80:
    print("Grade A")

elif marks >= 70:
    print("Grade B")

elif marks >= 60:
    print("Grade C")

else:
    print("Fail")
```

---

## Output

```text
Grade B
```