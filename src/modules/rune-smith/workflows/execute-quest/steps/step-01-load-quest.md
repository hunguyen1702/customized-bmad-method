---
name: step-01-load-quest
description: Read the Quest/Tech Spec
nextStepFile: './step-02-select-step.md'
quests_folder: '{project-root}/quests'
---

# Step 1: Load Quest

**Progress: Step 1 of 5** — Next: Select Step

## RULES

- Do not skip steps. Follow the sequence exactly.
- Speak output in `{communication_language}`.

## GOAL

Load the Quest file (Tech Spec) so you know the goal, steps, and acceptance criteria.

## SEQUENCE

### 1. Identify Quest File

If the user already provided a Quest path, use it. Otherwise ask:

"Which Quest should we execute? Please provide the path to the Quest file (e.g. `quests/quest-001-add-login.md`)."

### 2. Load and Read Quest

Read the full Quest file. Extract:

- **Goal**: What the feature/change is.
- **Steps**: Ordered implementation steps (with status if present).
- **Acceptance criteria**: How to verify.
- **stepsCompleted**: Which steps are already done (if any).

### 3. Summarize

Tell the user:

- Quest goal.
- Total steps and which (if any) are already complete.
- Next step to implement.

### 4. Continue

Present:

```
[Quest loaded. Ready to select next step.]

[C] Continue to Select Step
```

**HALT** and wait for **[C]**.

### 5. Proceed

When user selects **[C]**, load and execute **`steps/step-02-select-step.md`** in full. Pass the Quest path and content as context.
