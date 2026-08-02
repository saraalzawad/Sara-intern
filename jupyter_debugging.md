# Jupyter Debugging

## Common Debugging Techniques

### 1. Print Statements
Using `print()` is the easiest way to check variable values and see what the code is doing.

### 2. %debug
The `%debug` command helps inspect errors after a program stops because of an exception.

### 3. JupyterLab Debugger
The JupyterLab debugger lets you add breakpoints, check variables, and step through the code one line at a time.

### 4. %time and %timeit
These commands measure how long code takes to run and help find slow code.

# Summary

## What are the most common debugging techniques in notebooks?

The most common techniques are using `print()`, `%debug`, the JupyterLab debugger, and `%time` or `%timeit` to check performance.

## Which tools are most effective for the typical notebook workflow?

For most notebook work, `print()` is useful for simple checks, `%debug` helps find errors, and the JupyterLab debugger is helpful for larger programs.

## How do you debug harder notebook-specific issues?

If the notebook behaves strangely, I restart the kernel, run the cells again in order, and use the debugger or print statements to find the problem.