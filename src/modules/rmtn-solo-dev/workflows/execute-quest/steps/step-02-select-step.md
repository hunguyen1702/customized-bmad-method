---
name: step-02-select-step
description: Determine next step to implement
nextStepFile: './step-03-implement.md'
quests_folder: '{project-root}/quests'
---

# Step 2: Select Step

**Progress: Step 2 of 5** — Next: Implement

## RULES

- Do not skip steps. Follow the sequence exactly.
- Speak output in `{communication_language}`.

## GOAL

Determine which Quest step to implement next (first incomplete step, or user's choice).

## SEQUENCE

### 1. Determine Next Step

From the Quest file:

- If `stepsCompleted` exists, the next step is the first step not in that list.
- If no `stepsCompleted`, the next step is Step 1.

If the user wants to implement a specific step instead, allow that (e.g. "Implement step 3").

### 2. State the Step

Clearly state:

- Step number and description (from the Quest).
- Files and actions involved.
- Acceptance criteria for this step.

### 3. Confirm

Ask the user to confirm: "Ready to implement this step? [C] Continue to Implement."

**HALT** and wait for **[C]**.

### 4. Proceed

When user selects **[C]**, load and execute **`steps/step-03-implement.md`** in full. Pass the Quest path, current step index, and step details as context.
