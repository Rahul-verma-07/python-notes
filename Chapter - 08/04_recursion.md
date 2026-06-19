# Recursion in Python

Recursion is a programming technique in which a function calls itself.

It is often used to solve problems that can be broken down into smaller versions of the same problem.

Many mathematical formulas and algorithms can be implemented naturally using recursion.

---

# How Recursion Works

A recursive function performs two important tasks:

1. **Base Case** → The condition that stops the recursion.
2. **Recursive Case** → The part where the function calls itself.

Without a base case, the function would keep calling itself forever.

---

# Example: Factorial Using Recursion

The factorial of a number is defined as:

```text
n! = n × (n - 1)!
```

For example:

```text
5! = 5 × 4 × 3 × 2 × 1 = 120
```

---

## Program

```python
def factorial(n):

    if n < 0:
        return "Can't operate on negative numbers!"

    elif n == 0 or n == 1:
        return 1

    else:
        return n * factorial(n - 1)

num = int(input("Enter your number: "))

print(f"{num}! = {factorial(num)}")
```

---

## Sample Output

```text
Enter your number: 5

5! = 120
```

---

# Understanding the Recursive Calls

Suppose:

```python
factorial(5)
```

Python performs:

```text
factorial(5)
= 5 × factorial(4)

= 5 × (4 × factorial(3))

= 5 × (4 × (3 × factorial(2)))

= 5 × (4 × (3 × (2 × factorial(1))))

= 5 × 4 × 3 × 2 × 1

= 120
```

---

# Flow of Recursion

```text
factorial(5)
      │
      ▼
factorial(4)
      │
      ▼
factorial(3)
      │
      ▼
factorial(2)
      │
      ▼
factorial(1)
      │
      ▼
 Base Case Reached
      │
      ▼
 Return Backwards
      │
      ▼
 Final Answer
```

---

# Another Example

Print numbers from 5 to 1 using recursion:

```python
def countdown(n):

    if n == 0:
        return

    print(n)

    countdown(n - 1)

countdown(5)
```

---

## Output

```text
5
4
3
2
1
```

---

# Advantages of Recursion

- Makes code shorter and cleaner.
- Closely matches mathematical definitions.
- Useful for solving complex problems.
- Commonly used in tree and graph algorithms.

---

# Disadvantages of Recursion

- Uses more memory due to function calls.
- Can be slower than loops.
- May cause a stack overflow if recursion is too deep.

---

# Important Notes

> **NOTE:**
>
> - Every recursive function must have a **base case**.
> - The base case prevents infinite recursion.
> - Without a stopping condition, Python will keep calling the function until it raises a `RecursionError`.
> - Recursion is often the most direct and elegant way to implement certain algorithms.

---

# Infinite Recursion Example

```python
def hello():
    print("Hello")
    hello()

hello()
```

---

## Result

```text
RecursionError:
maximum recursion depth exceeded
```

### Explanation

The function keeps calling itself forever because there is no base case.

---

# Recursion vs Loop

| Recursion | Loop |
|------------|------------|
| Function calls itself | Repeats using loops |
| Requires a base case | Requires a condition |
| Easier for recursive problems | Usually more memory efficient |
| Can be more elegant | Often faster |

---

# Key Takeaway

Recursion is a technique where a function solves a problem by calling itself on a smaller version of the same problem, and it must always include a base case to stop the recursive calls.