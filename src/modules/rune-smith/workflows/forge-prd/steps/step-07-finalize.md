---
name: step-07-finalize
description: Mark PRD as complete and finish workflow
outputFile: '{output_folder}/prd-{project_name}.md'
---

# Step 7: Finalize

**Progress: Step 7 of 7** — Complete

## STEP GOAL:

Update the PRD status to complete and provide final summary to user.

## MANDATORY EXECUTION RULES (READ FIRST):

### Universal Rules:

- 📖 CRITICAL: Read complete step file before action
- 📋 YOU ARE A FACILITATOR
- ✅ Speak output in `{communication_language}`

### Step-Specific Rules:

- 🎯 Focus on clean completion
- 🚫 FORBIDDEN to make content changes
- 💬 Approach: Celebration and guidance

## EXECUTION PROTOCOLS:

- 🎯 Follow the MANDATORY SEQUENCE exactly
- 💾 Update PRD frontmatter status
- 📖 Provide next steps guidance

## CONTEXT BOUNDARIES:

- Available context: Approved PRD
- Focus: Status update and closure
- Output: Completed PRD

## MANDATORY SEQUENCE

**CRITICAL:** Follow this sequence exactly.

### 1. Update PRD Status

Update {outputFile} frontmatter:

```yaml
---
status: complete
stepsCompleted: ['step-01', 'step-02', 'step-03', 'step-04', 'step-05', 'step-06', 'step-07']
completedDate: '{current_date}'
---
```

### 2. Provide Completion Summary

```
**PRD Complete!** 🎉

**Document:** {outputFile}
**Status:** Complete
**Project Type:** {project_type}
**Tech Stack:** {language} / {framework}

**What's in the PRD:**
- Project Overview
- Target Users
- Requirements & Features

**Next Steps:**
- Use this PRD to guide development
- Reference it when making architectural decisions
- Update it as requirements evolve
```

### 3. Workflow Complete

```
**Forge PRD workflow complete.**

Thank you for using Mimir to forge your PRD, {user_name}!
```

---

## 🚨 SYSTEM SUCCESS/FAILURE METRICS

### ✅ SUCCESS:

- PRD status updated to 'complete'
- stepsCompleted array finalized
- User received completion summary
- Next steps guidance provided

### ❌ SYSTEM FAILURE:

- Leaving status as 'draft'
- Not updating frontmatter
- Missing completion message

**Master Rule:** Clean closure. PRD must be marked complete.
