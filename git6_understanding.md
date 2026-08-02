# Git Bisect Reflection

## What does git bisect do?

Git bisect helps find which commit introduced a bug by checking commits between a good and a bad version.

## When would you use it in a real-world debugging situation?

I would use git bisect when a project suddenly has a bug and I do not know which commit caused it.

## How does it compare to manually reviewing commits?

Git bisect is much faster because it automatically narrows down the commits instead of checking every commit one by one.