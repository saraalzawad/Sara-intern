# Advanced Git Commands

## What does each command do?

- `git checkout main -- <file>` restores a file from the main branch.
- `git cherry-pick <commit>` copies one commit from another branch.
- `git log` shows the commit history.
- `git blame <file>` shows who last changed each line in a file.

## When would you use these commands?

I would use `checkout` to restore a file, `cherry-pick` to copy a specific commit, `git log` to review previous commits, and `git blame` to find who changed a line of code and when.

## What surprised you while testing these commands?

I was surprised that Git can restore a single file without affecting the rest of the project. I also found `git blame` useful because it shows exactly who made each change.