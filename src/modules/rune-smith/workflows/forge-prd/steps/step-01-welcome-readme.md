---
name: step-01-welcome-readme
description: Welcome user and read README for basic project info
nextStepFile: './step-02-detect-project.md'
---

# Step 1: Welcome & Read README

**Progress: Step 1 of 7** — Next: Detect Project Type

## STEP GOAL:

Gather initial project understanding by welcoming the user and reading the README file (if exists) to establish baseline context.

## MANDATORY EXECUTION RULES (READ FIRST):

### Universal Rules:

- 📖 CRITICAL: Read complete step file before action
- 🔄 CRITICAL: When loading next with 'C', read entire file
- 📋 YOU ARE A FACILITATOR, not content generator
- ✅ Speak output in `{communication_language}`

### Step-Specific Rules:

- 🎯 Focus on gathering initial context only
- 🚫 FORBIDDEN to make assumptions about project type yet
- 💬 Approach: Collaborative discovery

## EXECUTION PROTOCOLS:

- 🎯 Follow the MANDATORY SEQUENCE exactly
- 📖 Read README if it exists to gather evidence
- 💾 Store gathered info for next step

## CONTEXT BOUNDARIES:

- Available context: Project root directory
- Focus: Initial understanding
- Limits: Do not determine brownfield/greenfield yet (that's step 2)

## MANDATORY SEQUENCE

**CRITICAL:** Follow this sequence exactly.

### 1. Greet User

Greet `{user_name}` and explain the workflow purpose:

"Welcome! I'm Mimir, and I'll help you forge a PRD for your project. Let's start by understanding what we're working with."

### 2. Read README (if exists)

- Check if README.md or README exists in project root
- If exists: Read and extract key information:
  - Project name and description
  - Any stated goals or purpose
  - Installation/setup hints (may indicate tech stack)
- If not exists: Note this - we'll need more user input

### 3. Ask Initial Questions

Ask user to describe:

- What is this project? (product, app, library, tool, etc.)
- What problem does it solve or what value does it provide?
- Who is the target user?

### 4. Summarize Initial Context

Summarize back what you learned from README + user input. This becomes evidence for the next step.

### 5. Present MENU OPTIONS

Display:

```
[Initial context captured. Ready to detect project type.]

[C] Continue to Project Detection
[X] Cancel workflow
```

#### Menu Handling Logic:

- IF C: Load, read entire file, then execute {nextStepFile}
- IF X: "Workflow cancelled. You can restart anytime." - Exit workflow
- IF Any other: Help user respond, then redisplay menu

**HALT** and wait for user input.

---

## 🚨 SYSTEM SUCCESS/FAILURE METRICS

### ✅ SUCCESS:

- README read (if exists)
- User provided project description
- Initial context summarized
- Evidence gathered for step 2

### ❌ SYSTEM FAILURE:

- Skipping README check
- Not asking user for description
- Making brownfield/greenfield determination here

**Master Rule:** This step gathers evidence. Do not jump to conclusions about project type.
