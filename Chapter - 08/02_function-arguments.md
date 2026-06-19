# Functions with Arguments in Python

Functions can accept values that they can work with.

These values are called **arguments** and are passed inside the parentheses when the function is called.

Arguments make functions more flexible and reusable.

---

# Function with Arguments

A function can receive data from the user or another part of the program through arguments.

---

## Syntax

```python
def function_name(argument):
    # Function Body

function_name(value)
```

---

## Example

```python
def greet(name):
    print(f"Good Day {name.capitalize()}")

name = input("Enter your name: ")

greet(name)
```

---

## Sample Output

```text
Enter your name: rahul
Good Day Rahul
```

### Explanation

- `name` inside the function definition is called a **parameter**.
- The value passed during the function call is called an **argument**.

```python
greet(name)
```

passes the user's name to the function.

---

# Multiple Arguments

A function can also accept multiple arguments.

## Example

```python
def add(a, b):
    print(a + b)

add(10, 20)
```

---

## Output

```text
30
```

---

# Default Parameter Value

We can assign a default value to a parameter.

If no argument is provided during the function call, Python uses the default value.

---

## Syntax

```python
def function_name(parameter="default_value"):
    # Function Body
```

---

## Example

```python
def greet(name="USER"):
    print("Hello " + name)

greet()
```

---

## Output

```text
Hello USER
```

### Explanation

Since no argument was passed:

```python
greet()
```

Python automatically uses:

```python
name = "USER"
```

---

# Example with Custom Argument

```python
def greet(name="USER"):
    print("Hello " + name)

greet("Rahul")
```

---

## Output

```text
Hello Rahul
```

### Explanation

The provided argument overrides the default value.

---

# Real-Life Example

```python
def welcome(name="Guest"):
    print(f"Welcome {name}")

welcome()
welcome("Rahul")
```

---

## Output

```text
Welcome Guest
Welcome Rahul
```

---

# Important Notes

> **NOTE:**
>
> - Parameters are variables written in the function definition.
> - Arguments are actual values passed during the function call.
> - Default parameters are used when no argument is provided.
> - A function can have multiple parameters.

---

# Difference Between Parameter and Argument

| Parameter | Argument |
|------------|------------|
| Defined inside the function | Passed during function call |
| Acts as a placeholder | Actual value supplied |
| Example: `name` | Example: `"Rahul"` |

### Example

```python
def greet(name):  # Parameter
    print(name)

greet("Rahul")    # Argument
```

---

# Key Takeaway

Arguments allow functions to work with different values, while default parameters provide a fallback value when no argument is supplied.