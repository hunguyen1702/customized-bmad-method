---
name: step-04-validate
description: Verify changes (lint/test)
nextStepFile: './step-05-update-status.md'
quests_folder: '{project-root}/quests'
---

# Step 4: Validate

**Progress: Step 4 of 5** — Next: Update Status

## RULES

- Do not skip steps. Follow the sequence exactly.
- Speak output in `{communication_language}`.

## GOAL

Verify the implementation: run lint and/or tests, and confirm the step meets acceptance criteria.

## SEQUENCE

### 1. Run Validation

- If the project has a linter, run it on the changed files (or the whole project).
- If the project has tests (unit/integration), run the relevant tests.
- If the Quest step has specific acceptance criteria, check them (e.g. manual check, script).

### 2. Report Results

- Report lint result (pass/fail, and any errors).
- Report test result (pass/fail, and any failures).
- If something failed, suggest fixes or ask the user how to proceed (fix and re-validate, or skip and continue).

### 3. Continue (when validation passes)

When validation passes (or user chooses to continue), present:

```
[Validation complete. Ready to update Quest status.]

[C] Continue to Update Status
```

**HALT** and wait for **[C]**.

### 4. Proceed

When user selects **[C]**, load and execute **`steps/step-05-update-status.md`** in full. Pass the Quest path and the step index that was completed.
