# Logical Operators in Python

Logical operators are used to build logic in Python programs.

They are mainly used to combine multiple conditions and return either:

```text
True
```

or

```text
False
```

Logical operators are commonly used with:

- `if` statements
- `if-else` statements
- `if-elif-else` statements
- Loops

to make decisions based on multiple conditions.

---

# Types of Logical Operators

| Operator | Meaning |
|----------|----------|
| `and` | Returns `True` if all conditions are `True` |
| `or` | Returns `True` if at least one condition is `True` |
| `not` | Reverses the Boolean value |

---

# 1. AND Operator

The `and` operator returns `True` only when all conditions are `True`.

---

## Example

```python
age = 20
has_id = True

print(age >= 18 and has_id)
```

---

## Output

```text
True
```

---

## Truth Table

| Condition 1 | Condition 2 | Result |
|------------|------------|---------|
| True | True | True |
| True | False | False |
| False | True | False |
| False | False | False |

---

# 2. OR Operator

The `or` operator returns `True` if at least one condition is `True`.

---

## Example

```python
marks = 35
sports_quota = True

print(marks >= 40 or sports_quota)
```

---

## Output

```text
True
```

---

## Truth Table

| Condition 1 | Condition 2 | Result |
|------------|------------|---------|
| True | True | True |
| True | False | True |
| False | True | True |
| False | False | False |

---

# 3. NOT Operator

The `not` operator reverses a Boolean value.

```text
True  → False
False → True
```

---

## Example

```python
is_logged_in = True

print(not is_logged_in)
```

---

## Output

```text
False
```

---

## Truth Table

| Value | Result |
|---------|---------|
| True | False |
| False | True |

---

# Example Using Logical Operators

```python
age = 20
has_id = True

if age >= 18 and has_id:
    print("Eligible to Vote")
```

---

## Output

```text
Eligible to Vote
```

---

# Real-Life Applications

Logical operators are used in:

- Login systems
- Voting eligibility checks
- ATM transactions
- Pass/Fail conditions
- Form validations
- Access control systems

---

# Important Note

Logical operators always return a Boolean value:

```python
True
```

or

```python
False
```

and help Python make decisions based on multiple conditions.