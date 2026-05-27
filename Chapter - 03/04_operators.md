# Operators in Python

Operators are special symbols used to perform operations on variables and values in Python.

---

# Types of Operators in Python

| Operator Type | Symbols | Uses |
|---|---|---|
| **Arithmetic Operators** | `+`, `-`, `*`, `/`, `%` | Used for calculations |
| **Assignment Operators** | `=`, `+=`, `-=` | Used to assign values |
| **Comparison Operators** | `==`, `>`, `<`, `>=`, `<=`, `!=` | Used to compare values |
| **Logical Operators** | `and`, `or`, `not` | Used to build logic |

---

# 1. Arithmetic Operators

Arithmetic operators are used to perform mathematical calculations.

## Example

```python
a = 7
b = 5

c = a + b

print(c)
```

## Output

```text
12
```

---

# 2. Assignment Operators

Assignment operators are used to assign or update values in variables.

## Example

```python
a = 4
a -= 2
# a = a - 2

b = 6
b += 3
# b = b + 3

print(a, b)
```

## Output

```text
2 9
```

---

# 3. Comparison Operators

Comparison operators compare two values and return either `True` or `False`.

## Example

```python
a = 1 == 1
b = 3 < 2
c = 2 > 3
d = 4 <= 5
e = 5 >= 4
f = 5 != 5

print(a)
print(b)
print(c)
print(d)
print(e)
print(f)
```

## Output

```text
True
False
False
True
True
False
```

---

# 4. Logical Operators

Logical operators are used to combine conditions and build logic.

The three logical operators are:

```text
and
or
not
```

---

# OR Operator

The `or` operator returns `True` if at least one condition is `True`.

## Example

```python
print("True or False is:", True or False)
print("True or True is:", True or True)
print("False or True is:", False or True)
print("False or False is:", False or False)
```

## Output

```text
True or False is: True
True or True is: True
False or True is: True
False or False is: False
```

---

# AND Operator

The `and` operator returns `True` only when both conditions are `True`.

## Example

```python
print("True and False is:", True and False)
print("True and True is:", True and True)
print("False and True is:", False and True)
print("False and False is:", False and False)
```

## Output

```text
True and False is: False
True and True is: True
False and True is: False
False and False is: False
```

---

# NOT Operator

The `not` operator reverses the Boolean value.

## Example

```python
a = True
b = False

print(not(a))
print(not(b))
```

## Output

```text
False
True
```

---

# Important Note

- Arithmetic operators work with numbers.
- Comparison operators always return `True` or `False`.
- Logical operators are mainly used in conditions and decision making.