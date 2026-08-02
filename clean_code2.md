# Commenting & Documentation

## Good Comment Example

### Before

```python
# do math
x = a + b
```

### After

```python
# Add the two numbers and store the result
total = first_number + second_number
```

## Reflection

### When should you add comments?
Comments should be added when the code is difficult to understand or when you need to explain why something was done. They are also useful for documenting functions and important parts of the code.

### When should you avoid comments and instead improve the code?
If the code can be made clear by using better variable names or smaller functions, it is better to improve the code instead of adding comments. Clear code is easier to read and needs fewer comments.

---------
# Handling Errors & Edge Cases

## Example

### Before

```python
def divide(a, b):
    return a / b
```

### After

```python
def divide(a, b):
    if b == 0:
        return "Error: Cannot divide by zero."
    return a / b
```

## Reflection

### What was the issue with the original code?
The original code did not check if the second number was zero. If someone entered zero, the program would crash with an error.

### How does handling errors improve reliability?
Handling errors makes the program more reliable because it can deal with invalid input without crashing. It also gives the user a clear message and makes the program easier to use.