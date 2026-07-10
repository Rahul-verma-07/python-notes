# File I/O in Python

File I/O (**Input/Output**) is used to read data from files and write data to files.

Since **RAM (Random Access Memory)** is a **volatile memory**, all the data stored in it is lost when the program terminates or the computer is turned off.

To store data permanently, we use **files**.

A **file** is a collection of data stored on a storage device such as a Hard Disk or SSD.

Python programs can interact with files by:

- Reading data from a file.
- Writing data to a file.

---

# Why Do We Need File I/O?

Without files, data exists only while the program is running.

Using File I/O allows us to:

- Store data permanently.
- Read previously saved information.
- Update existing data.
- Share data between different programs.

---

# Types of Files

Python mainly works with two types of files.

## 1. Text Files

Text files store data in the form of readable characters.

Common text file extensions include:

- `.txt`
- `.csv`
- `.py`
- `.html`
- `.json`

### Example

```text
student.txt
```

Contents:

```text
Rahul
18
Computer Science
```

---

## 2. Binary Files

Binary files store data in binary format (0s and 1s).

These files are not human-readable.

Common binary file extensions include:

- `.dat`
- `.bin`
- `.jpg`
- `.png`
- `.mp3`
- `.mp4`
- `.exe`

### Example

```text
image.jpg
video.mp4
data.bin
```

---

# Comparison Between Text and Binary Files

| Text Files | Binary Files |
|------------|--------------|
| Human-readable | Not human-readable |
| Stores characters | Stores binary data |
| Uses `.txt`, `.csv`, `.py` | Uses `.dat`, `.bin`, `.jpg`, `.mp4` |
| Easier to edit | Requires special software to view |

---

# Real-Life Applications

File I/O is commonly used for:

- Saving user information
- Maintaining student records
- Reading configuration files
- Logging program output
- Creating reports
- Storing application data

---

# Important Note

> **NOTE:**
>
> - Files help store data permanently.
> - Python provides built-in functions to read from and write to files.
> - Text files store readable data, whereas binary files store data in binary format.