# Appending to a File in Python

Python provides the `append()` mode (`"a"`) to add new data to the end of an existing file.

Unlike **Write Mode (`"w"`)**, Append Mode does **not** overwrite the existing contents of the file.

If the file does not exist, Python automatically creates it.

---

# Syntax

```python
file = open("file_name", "a")

file.write(data)

file.close()
```

---

# Example

```python
string = "\nKeep learning Python!"

file = open("my_file.txt", "a")

file.write(string)

file.close()

file = open("my_file.txt", "r")

data = file.read()

print(data)

file.close()
```

---

## Suppose `my_file.txt` Initially Contains

```text
Hey Rahul, you are amazing!
```

---

## Output

```text
Hey Rahul, you are amazing!
Keep learning Python!
```

---

# Explanation

```python
file = open("my_file.txt", "a")
```

- Opens the file in **Append Mode**.
- If the file does not exist, Python creates it.
- If the file already exists, Python keeps the existing contents.

```python
file.write(string)
```

- Adds the new data to the end of the file.

```python
file.close()
```

- Closes the file after writing.

```python
file = open("my_file.txt", "r")
```

- Opens the file in **Read Mode**.

```python
data = file.read()
```

- Reads the complete contents of the file.

```python
print(data)
```

- Displays the updated file contents.

---

# Flow of Appending to a File

```text
Open File (Append Mode)
          │
          ▼
      Existing Data
          │
          ▼
      Append New Data
          │
          ▼
       Close File
          │
          ▼
 Open File (Read Mode)
          │
          ▼
      Read Contents
          │
          ▼
      Display Output
```

---

# Difference Between Write and Append Mode

| Write Mode (`"w"`) | Append Mode (`"a"`) |
|---------------------|---------------------|
| Overwrites the existing file | Preserves existing data |
| Starts writing from the beginning | Writes at the end of the file |
| Creates the file if it doesn't exist | Creates the file if it doesn't exist |

---

# Example Comparison

### Write Mode (`"w"`)

Suppose the file contains:

```text
Hello World
```

```python
file = open("my_file.txt", "w")
file.write("Python")
file.close()
```

Result:

```text
Python
```

The previous data is removed.

---

### Append Mode (`"a"`)

Suppose the file contains:

```text
Hello World
```

```python
file = open("my_file.txt", "a")
file.write("\nPython")
file.close()
```

Result:

```text
Hello World
Python
```

The previous data remains unchanged.

---

# Summary

| Method | Purpose |
|----------|----------|
| `open("file.txt", "a")` | Opens a file in Append Mode |
| `write(data)` | Appends data to the end of the file |
| `close()` | Closes the file and saves changes |

---

# Important Notes

> **NOTE:**
>
> - `"a"` stands for **Append Mode**.
> - Existing data is never overwritten.
> - New data is always added at the end of the file.
> - If the file does not exist, Python creates it automatically.
> - Always close the file after appending data to ensure the changes are saved.

---

# Key Takeaway

Use **Append Mode (`"a"`)** when you want to add new information to an existing file without removing its current contents.