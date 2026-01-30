---
name: step-03-draft-updates
description: Propose changes to Saga files
nextStepFile: './step-04-review.md'
saga_folder: '{project-root}/_bmad/saga'
output_context: '{project-root}/_bmad/saga/context.md'
output_architecture: '{project-root}/_bmad/saga/architecture.md'
---

# Step 3: Draft Updates

**Progress: Step 3 of 5** — Next: Review

## RULES

- Do not skip steps. Follow the sequence exactly.
- Speak output in `{communication_language}`.

## GOAL

Produce draft updates for context.md and architecture.md based on the impact analysis (Step 2).

## SEQUENCE

### 1. Draft context.md Updates

- Start from the current context.md content.
- Apply the proposed PRD changes (add/change/remove sections).
- Keep the draft in memory or a WIP buffer; do not write to disk until Step 5.

### 2. Draft architecture.md Updates

- Start from the current architecture.md content.
- Apply the proposed architecture changes (add/change/remove sections).
- Keep the draft in memory or WIP; do not write to disk until Step 5.

### 3. Continue

Present:

```
[Saga updates drafted. Ready for review.]

[C] Continue to Review
```

**HALT** and wait for **[C]**.

### 4. Proceed

When user selects **[C]**, load and execute **`steps/step-04-review.md`** in full. Pass both drafts (context + architecture) into the next step.
