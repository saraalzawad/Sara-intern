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

----------------
# Code Formatting and Style Guides

## Why is code formatting important?
Code formatting makes code easier to read and understand. It helps developers follow the same style, which makes it easier to work together and maintain the code in the future.

## What issues did the linter detect?
The linter can find small problems like missing spaces, incorrect indentation, or unused variables. In my practice, I did not have any major issues, but I learned that a linter helps find mistakes before the code is shared.

## Did formatting make the code easier to read?
Yes. After formatting the code, it looked cleaner and more organized. It was easier to understand what each part of the code was doing, and I think it would also be easier for other developers to read.
------------------
# Naming Variables & Functions

## What makes a good variable or function name?
A good name should clearly explain what the variable or function does. It should be easy to understand and describe its purpose.

## What issues can arise from poorly named variables?
Poor variable names can make the code confusing and harder to read. They can also make it easier to make mistakes when changing the code later.

## How did refactoring improve code readability?
Changing names like `a`, `b`, and `c` to `first_number`, `second_number`, and `total` made the code much easier to understand. It was clear what each variable was used for.

## Example

### Before

```python
a = 5
b = 10
c = a + b
print(c)
```

### After

```python
first_number = 5
second_number = 10
total = first_number + second_number
print(total)
```
-------------------

# Writing Small, Focused Functions

## Why is breaking down functions beneficial?
Breaking a large function into smaller functions makes the code easier to read and understand. It also makes it easier to find and fix problems.

## Example

### Before

```python
def calculate_total(price, tax):
    total = price + tax
    print(total)
    print("Thank you for your purchase!")
```

### After

```python
def calculate_total(price, tax):
    return price + tax

def print_total(total):
    print(total)

def thank_customer():
    print("Thank you for your purchase!")
```

## How did refactoring improve the structure of the code?
After splitting the function into smaller parts, each function has one job. The code is more organized, easier to test, and easier to change later if needed.

-------
# Avoiding Code Duplication

## What is the DRY principle?
DRY stands for "Don't Repeat Yourself". It means we should avoid writing the same code more than once. Instead, we can reuse code by creating a function.

## Before

```python
print("Welcome")
print("Welcome")
print("Welcome")
```

## After

```python
def welcome():
    print("Welcome")

welcome()
welcome()
welcome()
```

## What were the issues with duplicated code?
Duplicated code makes the program longer and harder to maintain. If I need to change something, I have to update it in many places, which can lead to mistakes.

## How did refactoring improve maintainability?
By moving the repeated code into one function, the code became shorter, cleaner, and easier to update. If I want to change the message, I only need to change it in one place.