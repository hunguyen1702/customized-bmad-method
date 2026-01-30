---
name: step-04-review
description: User confirms updates
nextStepFile: './step-05-commit.md'
saga_folder: '{project-root}/_bmad/saga'
output_context: '{project-root}/_bmad/saga/context.md'
output_architecture: '{project-root}/_bmad/saga/architecture.md'
---

# Step 4: Review

**Progress: Step 4 of 5** — Next: Commit

## RULES

- Do not skip steps. Follow the sequence exactly.
- Speak output in `{communication_language}`.

## GOAL

Present the drafted Saga updates to the user and get approval or edits before writing to disk.

## SEQUENCE

### 1. Present Drafts

Show the user:

- The drafted **context.md** (full content or diff-style summary).
- The drafted **architecture.md** (full content or diff-style summary).

### 2. Ask for Feedback

Ask the user to:

- Approve as-is, or
- Request edits (add/change/remove).

### 3. Apply Edits

If the user requests changes, update the drafts and re-present until they are satisfied.

### 4. Confirm and Continue

When the user approves, present:

```
[Saga updates approved. Ready to write to disk.]

[C] Continue to Commit
```

**HALT** and wait for **[C]**.

### 5. Proceed

When user selects **[C]**, load and execute **`steps/step-05-commit.md`** in full. Ensure the approved drafts (context + architecture) are available to the final step.
