# Escape Sequence Characters in Python

Escape sequence characters are special characters used inside strings with a backslash `\`.

They are used to format text in different ways.

---

# Common Escape Sequence Characters

| Escape Sequence | Meaning |
|---|---|
| `\n` | New Line |
| `\t` | Tab Space |
| `\'` | Single Quote |
| `\"` | Double Quote |
| `\\` | Backslash |

---

# 1. New Line Character (`\n`)

The `\n` character is used to move the text to a new line.

## Example

```python
print("Hello\nWorld")
```

## Output

```text
Hello
World
```

---

# 2. Tab Character (`\t`)

The `\t` character is used to give tab space.

## Example

```python
print("Hello\tWorld")
```

## Output

```text
Hello    World
```

---

# 3. Single Quote (`\'`)

Used to insert a single quote inside a string.

## Example

```python
print('It\'s Python')
```

## Output

```text
It's Python
```

---

# 4. Double Quote (`\"`)

Used to insert double quotes inside a string.

## Example

```python
print("\"Python\"")
```

## Output

```text
"Python"
```

---

# 5. Backslash (`\\`)

Used to print a backslash character.

## Example

```python
print("Python\\Programming")
```

## Output

```text
Python\Programming
```

---

# Complete Example

```python
line = "Hey I am learning Python \\by my Mentor,\n\t\"Harish Ali Khan\""

print(line)
```

---

# Output

```text
Hey I am learning Python \by my Mentor,
    "Harish Ali Khan"
```

---

# Explanation

In the above example:

- `\\` prints a backslash `\`
- `\n` moves the text to a new line
- `\t` gives a tab space
- `\"` prints double quotes

---

# Important Note

Escape sequence characters are always written using a backslash `\`.

They are mainly used for:

- Formatting text
- Creating multi-line output
- Printing special characters inside strings