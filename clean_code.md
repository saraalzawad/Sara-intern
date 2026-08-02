# Clean Code Principles

Clean code means writing code that is easy to read and understand. It should be simple, organized, and use clear names. This makes it easier to fix problems and update the code later. For example, a=5 and b=10 are not clear, but first_number=5 and second_number=10 are much easier to understand. Clean code helps both you and other developers work with the code more easily.
---


## Messy Code

```python
a=5
b=10
c=a+b
print(c)
```

### Why difficult to read?
- Variable names are not meaningful.
- There are no comments.
- It does not clearly explain what the code is doing.

---

# Cleaner Version

```python
first_number = 5
second_number = 10
total = first_number + second_number

print(total)
```

### Why better?
- Variable names are clear.
- The code is easier to read.
- It is easier to understand and maintain.