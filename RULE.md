---
description: "Do not repeat yourself (DRY), a classic rule for reducing code duplication"
alwaysApply: true
---

# DRY Rule (Do Not Repeat Yourself)

DRY is the classic “Do Not Repeat Yourself” principle: **any knowledge, rule, or behavior should have a single authoritative representation in the codebase**.

Repetition isn’t just copying lines — it’s duplicating intent. When the same idea is encoded in multiple places, you create divergence risk. The first copy is a convenience; the second copy is a future bug.

## Guidelines

- If you see the same logic twice, extract it. The third time is already too late.
- Prefer one well‑named abstraction over many near‑duplicates.
- Centralize invariants and business rules at their natural boundary (domain model, service layer, core module).
- Don’t repeat “knowledge” in different forms (e.g., a validation rule in one file and a matching comment or test helper elsewhere). Make the code the source of truth.
- Avoid copy‑pasted conditionals with small edits; parameterize or compose instead.
- If two pieces of code look similar but are not truly the same concept, keep them separate — DRY is about shared intent, not forced sameness.
