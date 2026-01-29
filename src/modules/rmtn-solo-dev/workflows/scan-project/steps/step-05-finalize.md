---
name: step-05-finalize
description: Write Saga files to saga folder
saga_folder: '{project-root}/_bmad/saga'
output_context: '{project-root}/_bmad/saga/context.md'
output_architecture: '{project-root}/_bmad/saga/architecture.md'
---

# Step 5: Finalize

**Progress: Step 5 of 5** — Complete

## RULES

- Do not skip steps. Follow the sequence exactly.
- Speak output in `{communication_language}`.

## GOAL

Write the approved context.md and architecture.md to the Saga folder and close the workflow.

## SEQUENCE

### 1. Ensure Saga Folder Exists

Ensure the directory `{project-root}/_bmad/saga/` exists (create if needed).

### 2. Write context.md

Write the approved PRD content to `{project-root}/_bmad/saga/context.md`. Include frontmatter if desired, e.g.:

```yaml
---
stepsCompleted: [1, 2, 3, 4, 5]
---
```

### 3. Write architecture.md

Write the approved architecture content to `{project-root}/_bmad/saga/architecture.md`. Include frontmatter as appropriate.

### 4. Confirm Completion

Tell the user:

- Saga has been written to `_bmad/saga/context.md` and `_bmad/saga/architecture.md`.
- They can now use Thor for [NQ] New Quest or [EX] Execute Quest, and later [US] Update Saga when Quests are done.

Workflow complete.
