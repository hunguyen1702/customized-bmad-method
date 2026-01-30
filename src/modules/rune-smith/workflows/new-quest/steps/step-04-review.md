---
name: step-04-review
description: User reviews Tech Spec
nextStepFile: './step-05-create-quest.md'
---

# Step 4: Review

**Progress: Step 4 of 5** — Next: Create Quest

## RULES

- Do not skip steps. Follow the sequence exactly.
- Speak output in `{communication_language}`.

## GOAL

Present the Tech Spec to the user and get approval or edits before writing the Quest file.

## SEQUENCE

### 1. Present Tech Spec

Show the user the full Tech Spec (goal, approach, steps, acceptance criteria, dependencies).

### 2. Ask for Feedback

Ask the user to:

- Approve as-is, or
- Request edits (add/change/remove steps or criteria).

### 3. Apply Edits

If the user requests changes, update the Tech Spec and re-present until they are satisfied.

### 4. Confirm and Continue

When the user approves, present:

```
[Tech Spec approved. Ready to create Quest file.]

[C] Continue to Create Quest
```

**HALT** and wait for **[C]**.

### 5. Proceed

When user selects **[C]**, load and execute **`steps/step-05-create-quest.md`** in full. Ensure the approved Tech Spec is available to the final step.
