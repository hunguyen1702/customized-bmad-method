---
name: step-01-welcome-input
description: Get user description of the project
nextStepFile: './step-02-scan-codebase.md'
saga_folder: '{project-root}/_bmad/saga'
---

# Step 1: Welcome & Input

**Progress: Step 1 of 5** — Next: Scan Codebase

## RULES

- Do not skip steps. Follow the sequence exactly.
- Speak output in `{communication_language}`.

## GOAL

Understand the user's project in their words so you can scope the Saga (PRD + Architecture).

## SEQUENCE

### 1. Greet and Invite

Greet `{user_name}` and invite them to describe the project:

- What is this project? (product, app, library, etc.)
- Who is it for? What problem does it solve?
- Any existing docs or constraints to respect?

### 2. Capture Summary

Summarize back what you heard (scope, audience, main goals). Ask 1–2 clarifying questions if needed.

### 3. Confirm and Continue

When the user is satisfied with the scope, present:

```
[Saga scope confirmed. Ready to scan the codebase.]

[C] Continue to Scan Codebase
```

**HALT** and wait for user to select **[C]**.

### 4. Proceed to Next Step

When user selects **[C]**, update any in-memory state (e.g. `stepsCompleted: [1]`), then load and execute **`steps/step-02-scan-codebase.md`** in full.
