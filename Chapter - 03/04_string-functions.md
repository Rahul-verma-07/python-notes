# String Functions in Python

String functions are used to perform different operations on strings.

Some commonly used string functions in Python are:

1. `len()` Function
2. `.endswith()` Function
3. `.startswith()` Function
4. `.count()` Function
5. `.capitalize()` Function
6. `.find()` Function
7. `.replace()` Function

---

# 1. len() Function

The `len()` function returns the total length of a string.

---

## Example

```python
string = "Hello"

string_length = len(string)

print(string)
print(string_length)
```

---

## Output

```text
Hello
5
```

---

# 2. .endswith() Function

The `.endswith()` function checks whether a string ends with a given value or not.

It returns:

```text
True
```

or

```text
False
```

---

## Example

```python
string = "Hello"

end_string = string.endswith("llo")

print(string)
print(end_string)
```

---

## Output

```text
Hello
True
```

---

# 3. .startswith() Function

The `.startswith()` function checks whether a string starts with a given value or not.

---

## Example

```python
string = "Hello"

start_string = string.startswith("He")

print(string)
print(start_string)
```

---

## Output

```text
Hello
True
```

---

# 4. .count() Function

The `.count()` function counts the total number of occurrences of a character or word in a string.

---

## Example

```python
string = "Hello World"

char_count = string.count("o")

print(string)
print(char_count)
```

---

## Output

```text
Hello World
2
```

---

# 5. .capitalize() Function

The `.capitalize()` function converts the first character of a string into uppercase.

---

## Example

```python
string = "hello"

print(string.capitalize())
```

---

## Output

```text
Hello
```

---

# 6. .find() Function

The `.find()` function finds a word or character and returns the index of its first occurrence.

---

## Example

```python
string = "Hello World"

index = string.find("World")

print(string)
print(index)
```

---

## Output

```text
Hello World
6
```

### Explanation

```text
"W" of "World" is present at index 6.
```

---

# 7. .replace() Function

The `.replace()` function replaces an old word with a new word in a string.

---

## Example

```python
string = "Hello World"

replaced_string = string.replace("World", "Python")

print(string)
print(replaced_string)
```

---

## Output

```text
Hello World
Hello Python
```

---

# Important Note

Strings in Python are immutable.

This means:

```text
Strings cannot be changed permanently.
```

Functions create a new string instead of modifying the original string.

---

## Example

```python
string = "Hello World"

replaced_string = string.replace("World", "Python")

print(string)
print(replaced_string)
```

---

## Output

```text
Hello World
Hello Python
```

### Explanation

- Original string remains unchanged:

```python
"Hello World"
```

- A new modified string is created:

```python
"Hello Python"
```