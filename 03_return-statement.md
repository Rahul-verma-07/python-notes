# Return Statement in Python

The `return` statement is used to send a value back from a function.

When Python encounters a `return` statement, the function immediately ends and returns the specified value to the place where the function was called.

---

# Why Use return?

Functions often perform calculations or process data.

Instead of only printing the result, we can return the result and use it elsewhere in the program.

---

# Syntax

```python
def function_name():
    return value
```

---

# Example

```python
def greet(name="USER"):
    print("Hello " + name)

    return "Bye!"

a = greet()

print(a)
```

---

## Output

```text
Hello USER
Bye!
```

### Explanation

The function:

```python
return "Bye!"
```

returns the string `"Bye!"`.

The returned value is stored in:

```python
a = greet()
```

and later printed using:

```python
print(a)
```

---

# How return Works

```text
Function Call
      │
      ▼
 Function Executes
      │
      ▼
 return Value
      │
      ▼
 Value Sent Back
      │
      ▼
 Stored or Used
```

---

# Example: Returning a Sum

```python
def add(a, b):
    return a + b

result = add(10, 20)

print(result)
```

---

## Output

```text
30
```

---

# Example: Returning a Square

```python
def square(num):
    return num * num

print(square(5))
```

---

## Output

```text
25
```

---

# return vs print

Many beginners confuse `return` and `print`.

| print() | return |
|----------|----------|
| Displays output on the screen | Sends a value back from a function |
| Cannot be reused directly | Returned value can be stored and reused |
| Used for displaying information | Used for producing results |

---

## Example

```python
def func1():
    print("Hello")

def func2():
    return "Hello"

a = func2()

print(a)
```

---

## Output

```text
Hello
```

In `func2()`, the value is returned and can be stored in a variable.

---

# Multiple Statements After return

```python
def demo():
    return "Done"

    print("Hello")
```

The statement after `return` is never executed.

---

## Output

```text
Done
```

### Explanation

Once Python encounters:

```python
return
```

the function immediately terminates.

---

# Important Notes

> **NOTE:**
>
> - `return` ends the function immediately.
> - Any code written after `return` inside the function will not execute.
> - A function can return numbers, strings, lists, tuples, dictionaries, or any other Python object.
> - If no value is specified, Python returns `None` by default.

---

# Example: Returning Multiple Values

```python
def calculate(a, b):
    return a + b, a - b

sum_, difference = calculate(10, 5)

print(sum_)
print(difference)
```

---

## Output

```text
15
5
```

---

# Key Takeaway

The `return` statement allows a function to send results back to the caller, making functions more powerful, reusable, and useful in larger programs.