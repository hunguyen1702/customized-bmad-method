---
name: step-01-load-context
description: Read current Saga and completed Quest(s)
nextStepFile: './step-02-analyze-changes.md'
saga_folder: '{project-root}/_bmad/saga'
quests_folder: '{project-root}/quests'
---

# Step 1: Load Context

**Progress: Step 1 of 5** — Next: Analyze Changes

## RULES

- Do not skip steps. Follow the sequence exactly.
- Speak output in `{communication_language}`.

## GOAL

Load the current Saga (context.md, architecture.md) and the completed Quest(s) so you can determine what to update.

## SEQUENCE

### 1. Load Current Saga

Read:

- `{project-root}/_bmad/saga/context.md`
- `{project-root}/_bmad/saga/architecture.md`

If either is missing, inform the user they may need to run [SC] Scan Project first.

### 2. Identify Completed Quests

- List Quest files in the quests folder (or ask the user which Quest(s) were just completed).
- For each completed Quest, read the file and note: goal, steps completed, and any changes that affect PRD or architecture.

### 3. Summarize

Briefly summarize: current Saga scope and the completed Quest(s) that should be reflected in the Saga.

### 4. Continue

Present:

```
[Context loaded. Ready to analyze impact.]

[C] Continue to Analyze Changes
```

**HALT** and wait for **[C]**.

### 5. Proceed

When user selects **[C]**, load and execute **`steps/step-02-analyze-changes.md`** in full.
