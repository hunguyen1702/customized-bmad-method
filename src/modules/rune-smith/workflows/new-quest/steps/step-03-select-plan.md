---
name: step-03-select-plan
description: Select best approach and draft Tech Spec
nextStepFile: './step-04-review.md'
saga_folder: '{project-root}/_bmad/saga'
quests_folder: '{project-root}/quests'
---

# Step 3: Select & Plan

**Progress: Step 3 of 5** — Next: Review

## RULES

- Do not skip steps. Follow the sequence exactly.
- Speak output in `{communication_language}`.

## GOAL

Confirm the chosen approach and draft a detailed Tech Spec (implementation steps, files, acceptance criteria) for the Quest.

## SEQUENCE

### 1. Confirm Selection

If the user has not yet chosen an approach, ask them to pick one from the scored list. Record the chosen approach.

### 2. Draft Tech Spec

Produce a Tech Spec that includes:

- **Goal**: One-line summary of the feature/change.
- **Approach**: The selected approach and rationale.
- **Steps**: Ordered implementation steps (each with clear scope: files, actions).
- **Acceptance criteria**: How to verify the feature (Given/When/Then or checklist).
- **Dependencies**: Any prior work or constraints.

Keep the spec in memory or a WIP buffer; do not write to disk until Step 5.

### 3. Continue

Present:

```
[Tech Spec drafted. Ready for review.]

[C] Continue to Review
```

**HALT** and wait for **[C]**.

### 4. Proceed

When user selects **[C]**, load and execute **`steps/step-04-review.md`** in full. Pass the Tech Spec draft into the next step.
