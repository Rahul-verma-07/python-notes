# Writing to a File in Python

Python provides the `write()` method to write data into a file.

To write data, the file must be opened in **Write Mode (`"w"`)**.

If the file does not exist, Python automatically creates it.

If the file already exists, its previous contents are **overwritten**.

---

# Syntax

```python
file = open("file_name", "w")

file.write(data)

file.close()
```

---

# Example

```python
string = "Hey Rahul, you are amazing!"

file = open("my_file.txt", "w")

file.write(string)

file.close()

file = open("my_file.txt", "r")

data = file.read()

print(data)

file.close()
```

---

## Output

```text
Hey Rahul, you are amazing!
```

---

# Explanation

```python
file = open("my_file.txt", "w")
```

- Opens the file in **Write Mode**.
- If the file does not exist, Python creates it.
- If the file already exists, all previous data is erased.

```python
file.write(string)
```

- Writes the contents of the variable `string` into the file.

```python
file.close()
```

- Closes the file after writing.

```python
file = open("my_file.txt", "r")
```

- Opens the same file in **Read Mode**.

```python
data = file.read()
```

- Reads the contents of the file.

```python
print(data)
```

- Displays the file contents.

---

# Flow of Writing to a File

```text
Open File (Write Mode)
          │
          ▼
     Write Data
          │
          ▼
     Close File
          │
          ▼
Open File (Read Mode)
          │
          ▼
     Read Data
          │
          ▼
     Display Output
```

---

# Important Notes

> **NOTE:**
>
> - `"w"` stands for **Write Mode**.
> - If the file does not exist, Python creates it automatically.
> - If the file already exists, its previous contents are **overwritten**.
> - Always close the file after writing to save the changes.

---

# Example of Overwriting

Suppose `my_file.txt` contains:

```text
Hello World
```

Now execute:

```python
file = open("my_file.txt", "w")

file.write("Python")

file.close()
```

The file now contains:

```text
Python
```

The previous content:

```text
Hello World
```

has been completely removed.

---

# Summary

| Method | Purpose |
|---------|---------|
| `open("file.txt", "w")` | Opens a file in Write Mode |
| `write(data)` | Writes data to the file |
| `close()` | Closes the file and saves changes |

---

# Key Takeaway

Use **Write Mode (`"w"`)** when you want to create a new file or replace the existing contents of a file with new data.