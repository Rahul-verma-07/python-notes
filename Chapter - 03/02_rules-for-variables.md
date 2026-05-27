# Rules for Variable Names in Python

Variable names in Python must follow certain rules.

---

## Rules

### 1. Variable names can contain:

- Alphabets (`a-z`, `A-Z`)
- Digits (`0-9`)
- Underscore (`_`)

## Example

```python
name = "Rahul"
age1 = 18
student_name = "RV"
```

---

### 2. Variable names can start only with:

- An Alphabet
- An Underscore (`_`)

## Valid Examples

```python
name = "Rahul"
_student = "RV"
```

---

### 3. Variable names cannot start with a digit

## Invalid Example

```python
1name = "Rahul"
```

❌ This will produce an error.

---

### 4. Spaces are not allowed in variable names

## Invalid Example

```python
student name = "Rahul"
```

❌ Spaces are not allowed between variable names.

---

### 5. Special symbols are not allowed

Special symbols such as:

```text
@ # $ % ! &
```

cannot be used in variable names.

## Invalid Example

```python
name@ = "Rahul"
```

❌ This will produce an error.

---

# Valid Variable Names

```python
name = "Rahul"
_age = 18
student_name = "RV"
marks1 = 95
```

---

# Invalid Variable Names

```python
1name = "Rahul"
student name = "RV"
name@ = "Rahul"
```

---

# Important Note

Python variable names are **case-sensitive**.

This means:

```python
name
Name
NAME
```

are all considered different variables.