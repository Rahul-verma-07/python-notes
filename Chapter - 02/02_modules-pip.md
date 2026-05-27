# Modules in Python

A module is a file containing Python code written by someone else (usually) that can be imported and used in our programs.

Modules help programmers reuse code instead of writing everything from scratch.

## Examples of Modules

```python
Pyjokes
Flask
Django
```

---

# Importing Modules

Modules can be imported into a Python program using the `import` keyword.

## Syntax

```python
import module_name
```

## Example

```python
import pyjokes

joke = pyjokes.get_joke()
print(joke)
```

In the above example:

- `pyjokes` module is imported.
- `get_joke()` function is used to generate a joke.

---

# PIP in Python

`pip` is the package manager for Python.

It is used to install external modules using the terminal.

## Syntax

```bash
pip install module_name
```

## Example

```bash
pip install pyjokes
```

The above command installs the `pyjokes` module in Python.

---


# Types of Modules

There are two types of modules in Python:

## 1. Built-in Modules

These modules are already pre-installed in Python.

### Examples

```python
os
math
random
```

---

## 2. External Modules

These modules are not pre-installed and need to be installed using `pip`.

### Examples

```python
pyjokes
flask
django
```