---
name: step-03-analyze-draft
description: Draft context.md and architecture.md
nextStepFile: './step-04-review.md'
saga_folder: '{project-root}/_bmad/saga'
output_context: '{project-root}/_bmad/saga/context.md'
output_architecture: '{project-root}/_bmad/saga/architecture.md'
---

# Step 3: Analyze & Draft

**Progress: Step 3 of 5** — Next: Review

## RULES

- Do not skip steps. Follow the sequence exactly.
- Speak output in `{communication_language}`.

## GOAL

Produce first drafts of `context.md` (PRD) and `architecture.md` based on user input and codebase scan.

## SEQUENCE

### 1. Draft context.md (PRD)

Create a draft that includes:

- Project name and one-line description
- Goals and audience (from Step 1)
- High-level features/capabilities
- Out of scope (if any)

Write to a **draft in memory or a WIP buffer**; do not write to disk until Step 5 (Finalize).

### 2. Draft architecture.md

Create a draft that includes:

- Tech stack and key dependencies
- Directory/module structure summary
- Conventions (testing, config, entry points)
- No deep implementation detail—keep it high-level

Keep this draft in memory or WIP as well.

### 3. Continue

Present:

```
[Drafts ready for review.]

[C] Continue to Review
```

**HALT** and wait for **[C]**.

### 4. Proceed

When user selects **[C]**, load and execute **`steps/step-04-review.md`** in full. Pass the draft content (context + architecture) into the next step as context.
