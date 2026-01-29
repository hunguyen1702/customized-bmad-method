---
name: step-03-implement
description: Write code for the step
nextStepFile: './step-04-validate.md'
quests_folder: '{project-root}/quests'
---

# Step 3: Implement

**Progress: Step 3 of 5** — Next: Validate

## RULES

- Do not skip steps. Follow the sequence exactly.
- Speak output in `{communication_language}`.

## GOAL

Implement the selected Quest step: edit files, add/change code, and apply the changes.

## SEQUENCE

### 1. Implement the Step

- Read the step description and acceptance criteria from the Quest.
- Make the necessary code changes (create/edit/delete files as specified).
- Follow project conventions and the Tech Spec; keep changes minimal and reversible where possible.

### 2. Summarize Changes

Briefly list what was changed (files and main edits).

### 3. Continue

Present:

```
[Implementation complete. Ready to validate.]

[C] Continue to Validate
```

**HALT** and wait for **[C]**.

### 4. Proceed

When user selects **[C]**, load and execute **`steps/step-04-validate.md`** in full. Pass the Quest path, step index, and list of changed files as context.
