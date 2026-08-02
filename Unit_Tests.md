# Writing Unit Tests

## Testing Framework

I used **PyTest** because it is simple and commonly used for Python projects.

## Example Function

```python
def add(a, b):
    return a + b
```

## Unit Tests

```python
def test_add_positive():
    assert add(2, 3) == 5

def test_add_zero():
    assert add(5, 0) == 5

def test_add_negative():
    assert add(-2, -3) == -5
```

# Reflection

## How do unit tests help keep code clean?

Unit tests help make sure the code works correctly. They also make it easier to find bugs after making changes.

## What issues did you find while testing?

The tests helped me check different inputs, such as zero and negative numbers. I did not find any errors, but the tests showed that the function worked as expected.