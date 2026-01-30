---
name: step-05-create-quest
description: Write Quest file to quests folder
---

# Step 5: Create Quest

**Progress: Step 5 of 5** — Complete

## RULES

- Do not skip steps. Follow the sequence exactly.
- Speak output in `{communication_language}`.

## GOAL

Write the approved Tech Spec to a Quest file in the quests folder and close the workflow.

## SEQUENCE

### 1. Generate Quest ID and Slug

- **ID**: e.g. `quest-001` or based on date/sequence (ensure unique).
- **Slug**: Short name from the goal (e.g. `add-login`, `refactor-api`).

Filename pattern: `quest-{id}-{slug}.md` (e.g. `quest-001-add-login.md`).

### 2. Ensure Quests Folder Exists

Ensure the directory `{quests_folder}/` exists; create if needed.

### 3. Write Quest File

Write the Quest file to `{quests_folder}/quest-{id}-{slug}.md` with:

- **Frontmatter**: e.g. `title`, `slug`, `status: planned`, `stepsCompleted: []`, `created`, `goal`.
- **Body**: Goal, Approach, Steps (with checkboxes or status), Acceptance criteria, Dependencies.

Use the approved Tech Spec from Step 4.

### 4. Confirm Completion

Tell the user:

- Quest file path (e.g. `quests/quest-001-add-login.md`).
- They can run [EX] Execute Quest to implement it step-by-step.

Workflow complete.
