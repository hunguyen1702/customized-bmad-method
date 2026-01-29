---
name: step-05-update-status
description: Mark step complete in Quest file
quests_folder: '{project-root}/quests'
---

# Step 5: Update Status

**Progress: Step 5 of 5** — Complete (for this cycle)

## RULES

- Do not skip steps. Follow the sequence exactly.
- Speak output in `{communication_language}`.

## GOAL

Update the Quest file to mark the completed step (e.g. add to `stepsCompleted`, tick the step, or update status).

## SEQUENCE

### 1. Update Quest File

- Open the Quest file from context (path from Step 1).
- Update frontmatter: add the completed step index to `stepsCompleted` (e.g. `stepsCompleted: [1]` or `[1, 2]`).
- Optionally update the step in the body (e.g. mark as done, add a checkmark, or set status to "done").

### 2. Check if Quest is Complete

- If all steps are now in `stepsCompleted`, the Quest is fully implemented.
- If not, there are more steps to implement.

### 3. Tell the User

- Report: "Step N marked complete in Quest file."
- If the Quest is fully implemented: "Quest complete. All steps done. Consider running [US] Update Saga with Mimir to sync Saga."
- If more steps remain: "Next step to implement: Step N+1. Run [EX] Execute Quest again to continue, or ask me to implement the next step now."

Workflow cycle complete. User may run [EX] again to implement the next step or start a new Quest.
