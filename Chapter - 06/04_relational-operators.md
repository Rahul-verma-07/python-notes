# Relational Operators in Python

Relational operators are used to compare two values.

They evaluate a condition and return either:

```text
True
```

or

```text
False
```

Relational operators are commonly used inside:

- `if` statements
- `if-else` statements
- `if-elif-else` statements
- Loops

to make decisions in a program.

---

# Types of Relational Operators

| Operator | Meaning |
|----------|----------|
| `==` | Equal To |
| `<` | Less Than |
| `>` | Greater Than |
| `<=` | Less Than or Equal To |
| `>=` | Greater Than or Equal To |
| `!=` | Not Equal To |

---

# 1. Equal To (`==`)

Checks whether two values are equal.

## Example

```python
a = 10
b = 10

print(a == b)
```

---

## Output

```text
True
```

---

# 2. Less Than (`<`)

Checks whether the left value is smaller than the right value.

## Example

```python
a = 5
b = 10

print(a < b)
```

---

## Output

```text
True
```

---

# 3. Greater Than (`>`)

Checks whether the left value is greater than the right value.

## Example

```python
a = 20
b = 10

print(a > b)
```

---

## Output

```text
True
```

---

# 4. Less Than or Equal To (`<=`)

Checks whether a value is less than or equal to another value.

## Example

```python
a = 10
b = 10

print(a <= b)
```

---

## Output

```text
True
```

---

# 5. Greater Than or Equal To (`>=`)

Checks whether a value is greater than or equal to another value.

## Example

```python
a = 15
b = 10

print(a >= b)
```

---

## Output

```text
True
```

---

# 6. Not Equal To (`!=`)

Checks whether two values are different.

## Example

```python
a = 10
b = 20

print(a != b)
```

---

## Output

```text
True
```

---

# Using Relational Operators with if Statement

## Example

```python
age = 18

if age >= 18:
    print("Eligible to Vote")
```

---

## Output

```text
Eligible to Vote
```

---

# Important Note

Relational operators always return a Boolean value:

```python
True
```

or

```python
False
```

These values help Python make decisions during program execution.