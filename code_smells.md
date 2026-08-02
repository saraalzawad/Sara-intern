# Identifying & Fixing Code Smells

## Magic Numbers

### Before
```python
price = 100 * 0.1
```

### After
```python
DISCOUNT = 0.1
price = 100 * DISCOUNT
```

## Long Function

### Before
One function did everything.

### After
The function was split into smaller functions, and each one has one job.

## Duplicate Code

### Before
The same code was written in two places.

### After
The repeated code was moved into one function.

## Large Class

### Before
One class had too many responsibilities.

### After
The class was divided into smaller classes.

## Deeply Nested Conditionals

### Before
```python
if a:
    if b:
        if c:
            print("OK")
```

### After
```python
if a and b and c:
    print("OK")
```

## Commented-Out Code

### Before
```python
# print("Old code")
```

### After
The old commented code was removed.

## Inconsistent Naming

### Before
```python
x = 10
y = 20
```

### After
```python
width = 10
height = 20
```

# Reflection

### What code smells did you find in your code?
I found unclear variable names, repeated code, and some hardcoded values. These made the code harder to understand.

### How did refactoring improve the readability and maintainability of the code?
Refactoring made the code cleaner and easier to read. It also made it easier to change or update the code later.

### How can avoiding code smells make future debugging easier?
Clean code is easier to understand, so it is easier to find and fix bugs. It also helps other developers work with the code.