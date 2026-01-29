---
name: step-02-scan-codebase
description: Use tools to list and read key files
nextStepFile: './step-03-analyze-draft.md'
saga_folder: '{project-root}/_bmad/saga'
---

# Step 2: Scan Codebase

**Progress: Step 2 of 5** — Next: Analyze & Draft

## RULES

- Do not skip steps. Follow the sequence exactly.
- Speak output in `{communication_language}`.

## GOAL

List project structure and read key files (README, config, entry points, tests) to inform the Saga.

## SEQUENCE

### 1. List Structure

- List root directory and key folders (src, lib, app, tests, docs, etc.).
- Identify entry points, config files, and main modules.

### 2. Read Key Files

Read (or skim) as needed:

- README, package.json / requirements.txt / Cargo.toml (or equivalent)
- Main config files
- 1–2 main entry or core files to infer stack and patterns

### 3. Summarize Findings

Briefly summarize: tech stack, structure, and notable patterns. No drafting of Saga yet.

### 4. Continue

Present:

```
[Codebase scan complete. Ready to draft Saga.]

[C] Continue to Analyze & Draft
```

**HALT** and wait for **[C]**.

### 5. Proceed

When user selects **[C]**, load and execute **`steps/step-03-analyze-draft.md`** in full.
