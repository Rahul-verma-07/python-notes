# Functions in Python

A function is a group of statements that performs a specific task.

Functions help make programs more organized, readable, and reusable.

As programs grow larger and more complex, functions make it easier to manage code by breaking it into smaller logical parts.

---

# Why Use Functions?

Without functions, the same code may need to be written multiple times.

Functions allow us to:

- Reuse code
- Reduce repetition
- Improve readability
- Simplify debugging
- Organize large programs

---

# Function Definition

A function definition contains the set of instructions that will execute whenever the function is called.

---

## Syntax

```python
def function_name():
    # Function Body
```

---

## Example

```python
def func1():
    print("Hello")
```

In the above example:

- `def` is the keyword used to create a function.
- `func1` is the function name.
- The indented block is the function body.

---

# Function Call

A function call is used to execute a function.

Whenever we want to run a function, we write its name followed by parentheses `()`.

---

## Syntax

```python
function_name()
```

---

## Example

```python
func1()
```

---

# Complete Example

```python
# Function Definition

def greet():
    print("Hello World!")

# Function Call

greet()
```

---

## Output

```text
Hello World!
```

---

# How Functions Work

```text
Function Definition
         │
         ▼
Function Stored in Memory
         │
         ▼
   Function Call
         │
         ▼
 Function Executes
```

---

# Real-Life Example

Imagine a calculator program.

Instead of writing the addition code repeatedly, we can create a function:

```python
def add():
    print(10 + 20)
```

Now whenever we need addition:

```python
add()
```

---

# Important Notes

> **NOTE:**
>
> - A function must be defined before it is called.
> - A function can be called multiple times.
> - The function body executes only when the function is called.
> - Function names should be meaningful and descriptive.

---

# Example: Calling a Function Multiple Times

```python
def greet():
    print("Hello!")

greet()
greet()
greet()
```

---

## Output

```text
Hello!
Hello!
Hello!
```

---

# Summary

| Term | Description |
|--------|------------|
| Function | A reusable block of code |
| Function Definition | The code written inside a function |
| Function Call | Executes the function |
| `def` Keyword | Used to create a function |
| `()` | Used to call a function |

---

# Key Takeaway

Functions help us write cleaner, shorter, and more reusable code by grouping related statements into a single unit.