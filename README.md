# DRY

DRY: **Do Not Repeat Yourself**.

**Install**

```sh
pipx install cursorcult
cursorcult link DRY
```

Rule file format reference: https://cursor.com/docs/context/rules#rulemd-file-format

**When to use**

- You notice copy‑paste patterns or logic forks starting to drift.
- You want changes to a rule to happen in exactly one place.
- You’re building systems with stable invariants and business logic.

**What it enforces**

- Each rule/behavior has one authoritative implementation.
- Duplicated intent is treated as a defect to be refactored.
- Abstractions exist to remove repetition, not to increase it.

**Credits**

- Developed by Will Wieselquist. Anyone can use it.

**Origins**

- The DRY principle was coined by Andrew Hunt and David Thomas in *The Pragmatic Programmer* (1999): https://pragprog.com/titles/tpp20/the-pragmatic-programmer-20th-anniversary-edition/
