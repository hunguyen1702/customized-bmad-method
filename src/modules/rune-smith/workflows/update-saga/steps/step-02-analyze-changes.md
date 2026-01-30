---
name: step-02-analyze-changes
description: Determine impact on PRD/Arch
nextStepFile: './step-03-draft-updates.md'
---

# Step 2: Analyze Changes

**Progress: Step 2 of 5** — Next: Draft Updates

## RULES

- Do not skip steps. Follow the sequence exactly.
- Speak output in `{communication_language}`.

## GOAL

Determine how the completed Quest(s) affect the Saga: what should be added or changed in prd.md (PRD) and architecture.md.

## SEQUENCE

### 1. Impact on prd.md (PRD)

For each completed Quest:

- Does it add a new feature or capability? → Add or update the corresponding section in the PRD.
- Does it change scope or goals? → Update the goals/scope section.
- Does it affect "out of scope"? → Update if needed.

List proposed PRD changes (sections to add, change, or remove).

### 2. Impact on architecture.md

For each completed Quest:

- New components, modules, or tech? → Add or update the architecture section.
- New patterns or conventions? → Document them.
- Structural changes? → Update the structure description.

List proposed architecture changes (sections to add, change, or remove).

### 3. Continue

Present:

```
[Impact analyzed. Ready to draft Saga updates.]

[C] Continue to Draft Updates
```

**HALT** and wait for **[C]**.

### 4. Proceed

When user selects **[C]**, load and execute **`steps/step-03-draft-updates.md`** in full. Pass the list of proposed changes as context.
