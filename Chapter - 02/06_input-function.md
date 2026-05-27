# input() Function in Python

The `input()` function is used to take input from the user through the keyboard.

By default, the input taken using `input()` is stored as a **string** data type.

---

# Syntax

```python
input("Message")
```

---

# Example

```python
num = input("Enter your number: ")
# Input is taken as string

num_typecasted = int(input("Enter your num1: "))
# Input is type casted into integer

print(num)
print(type(num))

print(num_typecasted)
print(type(num_typecasted))
```

---

# Sample Output

```text
Enter your number: 7
Enter your num1: 10

7
<class 'str'>

10
<class 'int'>
```

---

# Explanation

## 1. Normal Input

```python
num = input("Enter your number: ")
```

- The value entered by the user is stored as a **string**.

Example:

```python
"7"
```

So:

```python
type(num)
```

returns:

```text
<class 'str'>
```

---

## 2. Type-Casted Input

```python
num_typecasted = int(input("Enter your num1: "))
```

- First, the input is taken as a string.
- Then it is converted into an integer using `int()`.

So:

```python
type(num_typecasted)
```

returns:

```text
<class 'int'>
```

---

# Important Note

By default:

```python
input()
```

always returns data in **string format**.

To use numbers for calculations, type casting is required.

---

# Example of Calculation

```python
a = int(input("Enter first number: "))
b = int(input("Enter second number: "))

print(a + b)
```

## Sample Output

```text
Enter first number: 5
Enter second number: 3

8
```