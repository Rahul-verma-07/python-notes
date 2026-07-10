# Opening and Reading a File in Python

Python provides the built-in `open()` function to open a file.

Before reading or writing a file, it must first be opened.

---

# Syntax

```python
file = open("file_name", "mode")
```

### Parameters

| Parameter | Description |
|------------|-------------|
| `file_name` | Name (or path) of the file to open |
| `mode` | Specifies how the file should be opened |

---

# Reading a File

After opening a file, the `read()` method is used to read its contents.

Once all operations are completed, the file should be closed using the `close()` method.

---

# Example

```python
file = open("file.txt", "r")

data = file.read()

print(data)

file.close()
```

---

## Sample File (`file.txt`)

```text
Hello World!
Welcome to Python File Handling.
```

---

## Output

```text
Hello World!
Welcome to Python File Handling.
```

---

# Explanation

```python
file = open("file.txt", "r")
```

- Opens the file named **file.txt**.
- `"r"` stands for **Read Mode**.

```python
data = file.read()
```

- Reads the entire content of the file.

```python
print(data)
```

- Displays the file contents on the screen.

```python
file.close()
```

- Closes the file and releases the resources.

---

# File Modes

| Mode | Description |
|------|-------------|
| `"r"` | Read a file (Default mode) |
| `"w"` | Write to a file (Creates a new file or overwrites an existing one) |
| `"a"` | Append data to a file |
| `"x"` | Create a new file (Raises an error if the file already exists) |
| `"b"` | Binary mode |
| `"t"` | Text mode (Default) |

---

# Flow of File Reading

```text
Open File
     │
     ▼
Read Content
     │
     ▼
Process / Print Data
     │
     ▼
Close File
```

---

# Important Notes

> **NOTE:**
>
> - Always close a file after completing the required operations.
> - If the specified file does not exist in **Read (`"r"`) mode**, Python raises a `FileNotFoundError`.
> - Reading a file does not modify its contents.
> - `"r"` is the default mode, so writing `open("file.txt")` is equivalent to `open("file.txt", "r")`.

---

# Example Using Default Read Mode

```python
file = open("file.txt")

print(file.read())

file.close()
```

The above program produces the same output as:

```python
file = open("file.txt", "r")
```