# Important Note

> **NOTE:**
>
> - There can be any number of `if` and `elif` statements in a program.
> - The `else` block is executed only when all the conditions in the `if` and `elif` statements evaluate to `False`.

---

## Example

```python
marks = 65

if marks >= 90:
    print("Grade A+")

elif marks >= 75:
    print("Grade A")

elif marks >= 60:
    print("Grade B")

else:
    print("Fail")
```

---

## Output

```text
Grade B
```

### Explanation

Python checks the conditions from top to bottom:

1. `marks >= 90` → False
2. `marks >= 75` → False
3. `marks >= 60` → True ✅

Since the third condition is `True`, Python executes:

```python
print("Grade B")
```

and skips the remaining conditions.

If all conditions had been `False`, the `else` block would have been executed.