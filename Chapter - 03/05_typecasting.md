# type() Function in Python

The `type()` function is used to find the data type of a variable in Python.

It tells us what kind of value a variable is storing.

---

# Syntax

```python
type(variable_name)
```

---

# Example

```python
a = 7
v = type(a)

b = 3.14
w = type(b)

c = "Rahul"
x = type(c)

d = True
y = type(d)

e = None
z = type(e)

print(v)
print(w)
print(x)
print(y)
print(z)
```

## Output

```text
<class 'int'>
<class 'float'>
<class 'str'>
<class 'bool'>
<class 'NoneType'>
```

---

# Explanation

| Variable | Value | Data Type |
|---|---|---|
| `a` | `7` | Integer (`int`) |
| `b` | `3.14` | Float (`float`) |
| `c` | `"Rahul"` | String (`str`) |
| `d` | `True` | Boolean (`bool`) |
| `e` | `None` | None Type (`NoneType`) |

---

# Type Casting in Python

Type Casting is a feature that allows us to convert one data type into another data type.

---

# Syntax

```python
new_data_type(variable)
```

---

# Example 1

```python
a = "3.14"
# Here "a" is a string

print(type(a))

# Type casting string into float
a = float(a)

print(type(a))
```

## Output

```text
<class 'str'>
<class 'float'>
```

---

# Example 2

```python
a = "3.14"

b = float(a)
# Here "b" stores the float value of variable "a"

t = type(b)

print(b)
print(t)
```

## Output

```text
3.14
<class 'float'>
```

---

# Common Type Casting Functions

| Function | Converts Into |
|---|---|
| `int()` | Integer |
| `float()` | Floating Point Number |
| `str()` | String |
| `bool()` | Boolean |

---

# Examples of Type Casting

## Integer to Float

```python
a = 7
b = float(a)

print(b)
```

## Output

```text
7.0
```

---

## Float to Integer

```python
a = 3.14
b = int(a)

print(b)
```

## Output

```text
3
```

---

## Integer to String

```python
a = 100
b = str(a)

print(type(b))
```

## Output

```text
<class 'str'>
```

---

# Important Note

- Type casting helps in changing data types when required.
- Some conversions may lose data.

For example:

```python
int(3.99)
```

returns:

```text
3
```

because the decimal part is removed.