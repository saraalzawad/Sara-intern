# Git Branching Reflection

## Why is pushing directly to `main` problematic?

Pushing directly to the `main` branch is risky because mistakes or bugs can affect the entire project immediately. Using a separate branch allows developers to test their changes before merging them into the main branch.

## How do branches help with reviewing code?

Branches make code reviews easier because each change is isolated. Team members can review the code, suggest improvements, and approve it before it is merged into the `main` branch.

## What happens if two people edit the same file on different branches?

If two people modify the same part of a file on different branches, Git may create a merge conflict when the branches are merged. The conflict must be resolved manually by deciding which changes should be kept.

This line was added in the main branch.