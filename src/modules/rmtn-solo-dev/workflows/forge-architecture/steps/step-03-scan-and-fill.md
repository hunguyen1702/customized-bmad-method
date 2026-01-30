---
name: 'step-03-scan-and-fill'
description: 'Scan codebase with 6 parallel sub-agents and fill architecture sections'

nextStepFile: './step-04-review.md'
outputFile: '{saga_folder}/architecture.md'
prdFile: '{saga_folder}/prd.md'
---

# Step 3: Scan & Fill

## STEP GOAL:

To analyze the codebase using **6 parallel sub-agents**, each responsible for filling one section of the architecture document. All agents work simultaneously for efficiency.

## MANDATORY EXECUTION RULES (READ FIRST):

### Universal Rules:

- 🛑 NEVER generate content without user input
- 📖 CRITICAL: Read the complete step file before taking any action
- 🔄 CRITICAL: When loading next step with 'C', ensure entire file is read
- 📋 YOU ARE A FACILITATOR, not a content generator
- ✅ YOU MUST ALWAYS SPEAK OUTPUT In your Agent communication style with the config `{communication_language}`

### Role Reinforcement:

- ✅ You are **Mimir** (God of Wisdom) - architecture analyst
- ✅ You orchestrate 6 sub-agents to work in parallel
- ✅ Each sub-agent focuses on ONE section only

### Step-Specific Rules:

- 🎯 Use 6 PARALLEL sub-agents for scanning
- 🔍 HIGH-LEVEL ONLY: Search keywords, pattern names - NO code snippets, NO file paths
- 🚫 FORBIDDEN to include specific file paths in output
- 🚫 FORBIDDEN to include code snippets in output
- 💬 Approach: Launch sub-agents → Aggregate results → Update document
- ⚙️ TOOL/SUBPROCESS FALLBACK: If sub-agents unavailable, perform sections sequentially in main thread

## EXECUTION PROTOCOLS:

- 🎯 Follow the MANDATORY SEQUENCE exactly
- 🔀 Launch 6 sub-agents in PARALLEL
- 💾 Each sub-agent updates its section in {outputFile}
- 📖 Update stepsCompleted when all sections filled

## CONTEXT BOUNDARIES:

- Available context: PRD from step 1, draft from step 2
- Focus: Codebase analysis and section filling
- Limits: HIGH-LEVEL ONLY - no code, no paths
- Dependencies: architecture.md draft exists

## CRITICAL PRINCIPLE: HIGH-LEVEL ONLY

⚠️ **READ THIS BEFORE SCANNING** ⚠️

The architecture document is a **thinking map**, not a **code index**.

| ❌ FORBIDDEN | ✅ REQUIRED |
|--------------|-------------|
| `src/services/auth_service.rb` | `*Service`, `auth`, `authenticate` |
| Code snippets | Pattern names and purposes |
| Implementation details | Search keywords for agents |
| Specific class names | Responsibility descriptions |

**Why?** Agents use keywords to SEARCH the codebase. They don't copy-paste paths.

## MANDATORY SEQUENCE

**CRITICAL:** Follow this sequence exactly. Do not skip, reorder, or improvise unless user explicitly requests a change.

### 1. Announce Scan Start

Display:
"**🔍 Bắt đầu Scan & Fill...**

Tôi sẽ deploy **6 sub-agents** để scan project song song:

| Agent | Section | Focus |
|-------|---------|-------|
| 🏗️ Agent 1 | High-Level Stack | Backend, DB, Async, Infra |
| 🗺️ Agent 2 | Logic & Feature Mapping | PRD → Keywords |
| 📊 Agent 3 | Data Model Strategy | Domain entities |
| 🔌 Agent 4 | API Interface Strategy | API types |
| ⚙️ Agent 5 | Coding Patterns | Patterns & keywords |
| 🧪 Agent 6 | Testing Strategy | Test stack |

**Đang scan...**"

### 2. Read PRD for Context

Load {prdFile} to extract:
- Project name
- Key features/requirements
- Any technical hints

This context guides all sub-agents.

### 3. Determine Search Strategy

Based on PRD and project structure, infer:
- Programming language (check file extensions)
- Package manager (package.json, Gemfile, requirements.txt, etc.)
- Framework hints from dependencies
- Directory structure patterns

### 4. Launch 6 Parallel Sub-Agents

**Launch ALL 6 sub-agents simultaneously:**

---

**SUB-AGENT 1: High-Level Stack**

*Mission:* Fill Section 1 with tech stack info

*Search for:*
- Package files (package.json, Gemfile, requirements.txt, go.mod, etc.)
- Config files (docker-compose, Dockerfile, .env.example)
- README for tech mentions

*Fill:*
- Backend framework
- Database
- Async processing (if any)
- Infrastructure hints

---

**SUB-AGENT 2: Logic & Feature Mapping**

*Mission:* Fill Section 2 - map PRD features to search keywords

*Process:*
1. List features from PRD
2. For EACH feature, identify search keywords (NOT paths!)
3. Add responsibility description

*Output format:*
```
| Feature | Search Keywords | Responsibility |
| Auth | `auth`, `session`, `login`, `jwt` | Manages user authentication |
```

---

**SUB-AGENT 3: Data Model Strategy**

*Mission:* Fill Section 3 with domain entities

*Search for:*
- Model/Entity definitions
- Database schema/migrations
- Type definitions

*Fill:*
- Core domain entities (abstracted, not table names)
- Entity relationships (conceptual)

---

**SUB-AGENT 4: API Interface Strategy**

*Mission:* Fill Section 4 with API types

*Search for:*
- Route definitions
- Controller/Handler patterns
- API documentation

*Categorize APIs by:*
- Public vs Private
- Admin vs User
- Webhooks
- Feature-specific groups

---

**SUB-AGENT 5: Coding Patterns & Search Strategy**

*Mission:* Fill Section 5 with patterns and search keywords

*Search for common patterns:*
- Service Objects (`*Service`, `*Manager`)
- Query Objects (`*Query`, `*Repository`)
- Form/Policy Objects (`*Policy`, `*Form`)
- Decorators/Presenters (`*Decorator`, `*Serializer`)
- Workers/Jobs (`*Worker`, `*Job`)

*For each pattern found, document:*
- Pattern name
- Purpose in this codebase
- Search keywords/suffixes

---

**SUB-AGENT 6: Testing Strategy**

*Mission:* Fill Section 6 with test stack

*Search for:*
- Test config files (jest.config, rspec, pytest.ini)
- Test directories structure
- Mock/stub patterns

*Document:*
- Test framework
- Data seeding approach
- External HTTP handling
- Coverage tools

---

### 5. Aggregate and Update Document

After all sub-agents complete:
1. Collect all section content
2. Update {outputFile} with filled sections
3. Update frontmatter:
   - Add 'step-03-scan-and-fill' to stepsCompleted
   - Update lastStep

### 6. Display Summary

Display:
"**✅ Scan & Fill hoàn tất!**

**Kết quả:**
- 📋 Section 1 (Stack): [summary]
- 🗺️ Section 2 (Features): [X features mapped]
- 📊 Section 3 (Data): [X entities]
- 🔌 Section 4 (APIs): [X API groups]
- ⚙️ Section 5 (Patterns): [X patterns]
- 🧪 Section 6 (Testing): [summary]

**Lưu ý:** Tất cả content đều ở mức HIGH-LEVEL (keywords, patterns).
Không có file paths hoặc code snippets.

**Tiếp theo:** Review document với bạn."

### 7. Present MENU OPTIONS

Display: "**Select:** [C] Continue to Review"

#### Menu Handling Logic:

- IF C: Update {outputFile} frontmatter, then load, read entire file, then execute {nextStepFile}
- IF Any other: Answer questions, then redisplay menu

#### EXECUTION RULES:

- ALWAYS halt and wait for user input after presenting menu
- ONLY proceed to next step when user selects 'C'
- User may ask questions about scan results before continuing

## CRITICAL STEP COMPLETION NOTE

ONLY WHEN user selects 'C' and document is updated will you load `./step-04-review.md` for user review.

---

## 🚨 SYSTEM SUCCESS/FAILURE METRICS

### ✅ SUCCESS:

- All 6 sections filled with HIGH-LEVEL content
- No file paths in output
- No code snippets in output
- Search keywords provided for each feature/pattern
- Document updated with stepsCompleted
- User can proceed to review

### ❌ SYSTEM FAILURE:

- Including specific file paths (e.g., `src/services/auth.rb`)
- Including code snippets
- Missing any of the 6 sections
- Running sub-agents sequentially when parallel is possible
- Not using search keywords format

**Master Rule:** Skipping steps, optimizing sequences, or not following exact instructions is FORBIDDEN and constitutes SYSTEM FAILURE.
