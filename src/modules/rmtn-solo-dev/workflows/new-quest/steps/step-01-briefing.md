---
name: step-01-briefing
description: Get user request and read Saga
nextStepFile: './step-02-strategize.md'
saga_folder: '{project-root}/_bmad/saga'
quests_folder: '{project-root}/quests'
---

# Step 1: Briefing

**Progress: Step 1 of 5** — Next: Strategize

## RULES

- Do not skip steps. Follow the sequence exactly.
- Speak output in `{communication_language}`.

## GOAL

Understand the user's feature request and load the Saga (context.md, architecture.md) so you can plan the Quest.

## SEQUENCE

### 1. Load Saga

Load and read (if they exist):

- `{project-root}/_bmad/saga/context.md`
- `{project-root}/_bmad/saga/architecture.md`

If either is missing, inform the user they may need to run [SC] Scan Project with Mimir first.

### 2. Get User Request

Ask `{user_name}` what feature or change they want to plan. Capture:

- What should be built or changed?
- Any constraints or priorities?

### 3. Confirm Scope

Summarize back the request and scope. Ask 1–2 clarifying questions if needed.

### 4. Continue

When scope is clear, present:

```
[Request and Saga loaded. Ready to brainstorm approaches.]

[C] Continue to Strategize
```

**HALT** and wait for **[C]**.

### 5. Proceed

When user selects **[C]**, load and execute **`steps/step-02-strategize.md`** in full.
