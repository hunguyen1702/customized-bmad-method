---
name: step-04-review
description: Present drafts to user for approval
nextStepFile: './step-05-finalize.md'
saga_folder: '{project-root}/_bmad/saga'
---

# Step 4: Review

**Progress: Step 4 of 5** — Next: Finalize

## RULES

- Do not skip steps. Follow the sequence exactly.
- Speak output in `{communication_language}`.

## GOAL

Present the draft context.md and architecture.md to the user and get approval or edits before writing to disk.

## SEQUENCE

### 1. Present Drafts

Show the user:

- The full draft of **context.md** (PRD).
- The full draft of **architecture.md**.

### 2. Ask for Feedback

Ask the user to:

- Approve as-is, or
- Request specific edits (sections to add, change, or remove).

### 3. Apply Edits (if any)

If the user requests changes, update the drafts accordingly and re-present until they are satisfied.

### 4. Confirm and Continue

When the user approves, present:

```
[Saga drafts approved. Ready to write to disk.]

[C] Continue to Finalize
```

**HALT** and wait for **[C]**.

### 5. Proceed

When user selects **[C]**, load and execute **`steps/step-05-finalize.md`** in full. Ensure the approved draft content (context + architecture) is available to the finalize step.
