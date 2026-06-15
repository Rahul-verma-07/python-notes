# Nested if Statement in Python

A Nested `if` statement means placing one `if` statement inside another `if` statement.

It is used when a second condition needs to be checked only if the first condition is `True`.

---

# Syntax

```python
if condition1:

    if condition2:
        print("Condition 2 is True")

    else:
        print("Condition 2 is False")

else:
    print("Condition 1 is False")
```

---

# How it Works

1. Python first checks the outer `if` condition.
2. If the outer condition is `True`, Python enters the nested `if` block.
3. Then Python checks the inner condition.
4. Based on the result, the corresponding block is executed.

---

# Example 1

```python
age = 20
has_id = True

if age >= 18:

    if has_id:
        print("Eligible to Vote")

    else:
        print("ID Card Required")

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
marks = 85

if marks >= 40:

    if marks >= 75:
        print("Passed with Distinction")

    else:
        print("Passed")

else:
    print("Failed")
```

---

## Output

```text
Passed with Distinction
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
   Condition 2      Execute
         │          else Block
    ┌────┴────┐
    │         │
  True      False
    │         │
 Execute   Execute
 Block     Block
```

---

# Real-Life Example

Suppose a student wants admission to a course.

Conditions:

1. Student must pass the entrance exam.
2. Student must submit the required documents.

```python
passed_exam = True
submitted_documents = True

if passed_exam:

    if submitted_documents:
        print("Admission Confirmed")

    else:
        print("Submit Documents")

else:
    print("Admission Rejected")
```

---

## Output

```text
Admission Confirmed
```

---

# Important Note

- A Nested `if` statement is simply an `if` inside another `if`.
- It is useful when one condition depends on another condition.
- Proper indentation is very important in nested statements.

---

# Difference Between if-else and Nested if

| if-else | Nested if |
|----------|----------|
| Checks one condition at a time | Checks conditions inside conditions |
| Simpler structure | More detailed decision making |
| Used for basic decisions | Used for dependent decisions |