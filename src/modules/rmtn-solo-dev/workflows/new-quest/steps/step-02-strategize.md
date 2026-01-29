---
name: step-02-strategize
description: Brainstorm 3 approaches and score them
nextStepFile: './step-03-select-plan.md'
saga_folder: '{project-root}/_bmad/saga'
quests_folder: '{project-root}/quests'
---

# Step 2: Strategize

**Progress: Step 2 of 5** — Next: Select & Plan

## RULES

- Do not skip steps. Follow the sequence exactly.
- Speak output in `{communication_language}`.

## GOAL

Brainstorm at least 3 implementation approaches and score them (Risk, Impact, Ease) so the user can choose the best one.

## SEQUENCE

### 1. Brainstorm Approaches

Propose at least 3 distinct approaches to implement the feature (from Step 1). For each:

- Brief description
- Pros and cons
- Rough effort/complexity

### 2. Score Each Approach

For each approach, score (e.g. 1–5 or Low/Medium/High):

- **Risk**: How much could go wrong? (e.g. regressions, unknowns)
- **Impact**: How well does it meet the goal?
- **Ease**: How simple to implement and maintain?

Present the table to the user.

### 3. Recommend (Optional)

Optionally recommend one approach based on the scores and project context. Do not decide for the user.

### 4. Continue

Present:

```
[Approaches scored. Ready to select and draft Tech Spec.]

[C] Continue to Select & Plan
```

**HALT** and wait for **[C]**.

### 5. Proceed

When user selects **[C]**, load and execute **`steps/step-03-select-plan.md`** in full. Pass the chosen approach (or user's choice) into the next step.
