---
name: step-05-consolidate-draft
description: Consolidate gathered information into PRD draft following template structure
nextStepFile: './step-06-review-cycle.md'
outputFile: '{output_folder}/prd-{project_name}.md'
prdTemplate: '../templates/prd-template.md'
---

# Step 5: Consolidate Draft

**Progress: Step 5 of 7** — Next: Review Cycle

## STEP GOAL:

Consolidate all information gathered from previous steps into the PRD draft, following the template structure. Transform raw information into a coherent, user-focused PRD document.

## MANDATORY EXECUTION RULES (READ FIRST):

### Universal Rules:

- 📖 CRITICAL: Read complete step file before action
- 🔄 CRITICAL: When loading next with 'C', read entire file
- 📋 YOU ARE A FACILITATOR working with user input
- ✅ Speak output in `{communication_language}`
- 🚫 CRITICAL: NO code or technical information in the PRD

### Step-Specific Rules:

- 🎯 Focus on consolidating and structuring information
- 🚫 FORBIDDEN to add technical/code details
- 🚫 FORBIDDEN to invent information not provided by user
- 💬 Approach: Synthesize and organize existing information

## EXECUTION PROTOCOLS:

- 🎯 Follow the MANDATORY SEQUENCE exactly
- 📖 Reference template for structure
- 💾 Write consolidated content to {outputFile}
- 🔄 Preserve user's voice and intent

## CONTEXT BOUNDARIES:

- Available context: Information from steps 1-4, PRD template
- Focus: Structure and consolidate (business context only)
- Limits: Do not add new information without user confirmation

## MANDATORY SEQUENCE

**CRITICAL:** Follow this sequence exactly.

### 1. Review Template Structure

Read {prdTemplate} to understand the target structure:

- Section 1: Title
- Section 2: Project Overview
- Section 3: Target User
- Section 4: Requirements & Features

### 2. Gather Information from Previous Steps

Recall information gathered:

**From Step 1 (Welcome/README):**
- Project name and description
- Initial project context
- User's description of the project

**From Step 2 (Detect Project):**
- Project type (greenfield/brownfield)
- Basic categorization

**From Step 3 (Placeholder):**
- PRD file created with frontmatter

**From Step 4 (Scan - if brownfield):**
- Core features identified (user perspective)
- User interactions
- External integrations (from user perspective)

### 3. Map Information to Template Sections

For each section, synthesize the gathered information:

**Section 2: Project Overview**
- What: System type and core problem it solves
- How: Key solution/mechanism (from user perspective, NOT technical)
- Why: Primary goal and value proposition

**Section 3: Target User**
- Who: Primary user roles
- What they do: Main objectives and interactions

**Section 4: Requirements & Features**
- Group features by user-facing functionality
- Describe each feature from user perspective
- NO implementation details

### 4. Write Consolidated Draft

Update {outputFile} with consolidated content:

"**Consolidating PRD draft...**

I'm now organizing all the information we've gathered into a structured PRD document."

**Write each section to the PRD file:**
- Replace template placeholders with actual content
- Maintain consistent tone and language
- Keep focus on business/user perspective

### 5. Present Draft Summary

After writing, present a summary:

"**PRD Draft Consolidated**

📄 **File:** {outputFile}

**Sections Completed:**
- ✅ Title: {project_name}
- ✅ Project Overview: [brief summary]
- ✅ Target User: [user types identified]
- ✅ Requirements & Features: [feature count] features across [group count] groups

**Key Points Captured:**
- [Point 1]
- [Point 2]
- [Point 3]

The draft is ready for your review in the next step."

### 6. Present MENU OPTIONS

Display:

```
[PRD draft consolidated. Ready for review.]

[C] Continue to Review Cycle
[P] Preview full draft now
[X] Cancel workflow
```

#### Menu Handling Logic:

- IF C: Update stepsCompleted in frontmatter, then load, read entire file, then execute {nextStepFile}
- IF P: Display full PRD content, then redisplay menu
- IF X: "Workflow paused. Your draft is saved at {outputFile}." - Exit workflow
- IF Any other: Help user respond, then redisplay menu

**HALT** and wait for user input.

---

## 🚨 SYSTEM SUCCESS/FAILURE METRICS

### ✅ SUCCESS:

- Template structure followed
- All gathered information consolidated
- Content written to PRD file
- NO technical/code details included
- User-focused language throughout
- Summary presented to user

### ❌ SYSTEM FAILURE:

- Including technical implementation details
- Adding information not provided by user
- Skipping template structure
- Not writing to output file
- Using developer-centric language

**Master Rule:** Consolidate existing information into structured format. Business/user focus only. No technical details.
