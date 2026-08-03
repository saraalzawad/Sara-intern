# Writing Meaningful Commit Messages

## What makes a good commit message?

A good commit message is short, clear, and explains what changed. It should help other people understand the purpose of the commit without reading all of the code.

## How does a clear commit message help in team collaboration?

A clear commit message helps team members understand changes quickly. It makes it easier to review code, find specific changes, and understand the project's history.

## How can poor commit messages cause issues later?

Poor commit messages can make it difficult to know what was changed or why it was changed. This can make debugging, reviewing code, and finding bugs much harder.

---

# Commit Message Best Practices

After researching commit messages, I learned these best practices:

- Keep the message short and clear.
- Explain what changed.
- Start with an action word such as **Add**, **Fix**, **Update**, or **Remove**.
- Make each commit focus on one change.
- Avoid unclear messages like **update**, **fix**, or **fixed stuff**.

---

# Open-Source Commit History Analysis

I looked at the commit history of the React project on GitHub and compared good and bad commit messages.

## Good commit message examples

### Example 1

```
Fix typo in documentation
```

**Why it is good:**

- It clearly explains what was fixed.
- It is short and easy to understand.

### Example 2

```
Add support for new API option
```

**Why it is good:**

- It starts with an action word.
- It explains exactly what was added.

## Bad commit message examples

### Example 1

```
update
```

**Why it is bad:**

- It does not explain what was updated.
- Other developers will not know what changed.

### Example 2

```
fix
```

**Why it is bad:**

- It is too short.
- It does not explain what was fixed or why.

---

# My Commit Message Practice

For this task, I created three commits using different styles:

1. **Vague commit message**
   - `fixed stuff`

2. **Very detailed commit message**
   - `Updated git5_understanding.md by adding another practice line to demonstrate a very detailed commit message for the internship Git exercise`

3. **Well-structured commit message**
   - `Add Git commit message reflection`

After this exercise, I understand that a good commit message should be clear, meaningful, and easy for other developers to understand.