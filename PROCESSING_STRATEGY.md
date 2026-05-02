# Processing Strategy

This document defines the efficient, lateral, function-based strategy for processing the remaining Obsidian vault material.

Use together with:
- `ARCHITECTURE.md`
- `RETENTION_POLICY.md`
- `01_STAGING/PROCESSING_AUDIT.md`
- `CODEX.md`
- `09_TEMPLATES/`

## 1. Objective

Convert the remaining vault into a practical second brain optimized for:
- retrieval
- reuse
- revision
- execution
- source traceability
- future expansion

The goal is not to maximize note count. The goal is to convert raw material into the smallest useful set of source-backed, linked, practical artifacts.

## 2. Core principle

Process by function first, folder second.

A folder is a safe processing boundary, but many useful concepts are scattered across folders. When duplicate or related material is obvious, process by explicitly named cross-folder clusters.

## 3. Processing lanes

### Lane A — Source preservation
For PDFs, DOCX, ZIPs, raw exports, book/article notes, large guides.

Default outputs:
- `05_REFERENCES/`
- attachment indexes
- source registers

Rule:
Do not decompose source material wholesale. Extract only high-value reusable ideas.

### Lane B — Reusable knowledge
For concepts, heuristics, principles, definitions, lessons, mental models.

Default outputs:
- `02_ATOMIC_NOTES/`
- `07_MODELS/`
- `03_MAPS_OF_CONTENT/`

Rule:
Create atomic notes only when the idea is reusable outside the original source.

### Lane C — Execution systems
For checklists, routines, job search plans, interview prep, learning plans, action systems.

Default outputs:
- `04_PROJECTS/`
- `07_MODELS/`
- `08_DECISIONS/`
- executable checklists/protocols

Rule:
Convert guides and checklists into usable protocols, not summaries.

### Lane D — Journal / reflection
For identity, emotion, personal reflection, character studies, values, commitments.

Default outputs:
- `06_JOURNAL/`

Rule:
Protect original personal meaning. Extract atomic/model notes only when a reusable principle is clearly present.

### Lane E — Retrieval / indexing
For MOCs, dashboards, lists, resource hubs, registers.

Default outputs:
- `03_MAPS_OF_CONTENT/`
- `05_REFERENCES/`

Rule:
MOCs must improve retrieval. Do not create decorative hubs.

## 4. Source classification and transformation rules

| Source type | Transformation |
|---|---|
| Raw idea | Atomic note only if reusable; otherwise staging/open-loop note |
| List/register | Reference register or MOC; avoid over-atomicization |
| Guide | Reference note plus practical checklist/model if useful |
| Checklist | Executable protocol or project checklist |
| Project/action material | Project note, task system, decision log, or action plan |
| Model/framework | Model note with meaning, use trigger, algorithm, failure modes |
| Journal/reflection | Journal note; preserve original; cautious extraction only |
| Source/reference | Reference note/register; preserve source |
| Duplicate/variant | Canonicalization recommendation, aliases, retention candidate |
| Placeholder | needs-review, empty-placeholder, or trash candidate |
| Binary attachment | Attachment index first; selective extraction later |

## 5. Folder-first vs cluster-first decision rule

Use folder-first when:
- folder is small
- content is homogeneous
- no obvious duplicates exist elsewhere
- processing objective is clear

Use cluster-first when:
- duplicate or variant files are obvious
- one concept appears across multiple folders
- processing one folder alone would create fragmented outputs
- there is a mature MOC/model/project that should become canonical

Cross-folder cluster constraint:
Every source file must be explicitly named in the task. Do not say “process all related notes” without a file list.

## 6. Mandatory batch lifecycle

Every substantial batch follows:

1. Processing
2. Quality review
3. Corrections
4. Quality review v2
5. Retention actions
6. Next batch

No retention before corrections. No new batch before the prior batch is safe to proceed or explicitly paused.

## 7. Remaining recommended sequence

### Phase 0 — Close current open batch
1. LISTS corrections
2. LISTS quality-review-v2
3. LISTS retention actions

### Phase 1 — SYSTEMS clusters
Process `01_STAGING/01_LONG_FORM/SYSTEMS/` by clusters:

#### 1A. Habit / routine / time architecture
Suggested files:
- `1. How to Create a Routine.md`
- `How to Create a Routine.md`
- `Daily Rhythm and Routine.md`
- `Daily_Rhythm_System.md`
- `Time Blocking.md`
- `Time_Architecture.md`
- `Daily Shutdown Ritual.md`
- `Digital Sunset.md`

Likely outputs:
- daily rhythm model
- personal operating system project
- time architecture protocol
- MOC links to attention/productivity

#### 1B. Procrastination / habit mechanics
Suggested files:
- `2-Minute Rule.md`
- `Micro Habits.md`
- `Procrastination Framework.md`
- `Seinfeld Strategy.md`
- `Snowballing.md`
- `How to Avoid Craving and Procrastination.md`
- `Action and Productivity.md`
- `Changing Myself & Following This in Life.md`

Likely outputs:
- anti-procrastination model
- habit-change protocol
- behavior-change project/checklist

#### 1C. Flow / focus systems
Suggested files:
- `K Step for Flow.md`
- `K-Step Guide to Flow.md`
- `Pomodoro Technique.md`
- `Hunter Method.md`
- `5 AM Club.md`

Optionally include explicitly named matching NOTES files later:
- `Flow State.md`
- `Flow_State.md`
- `Flow Cycle.md`

Likely outputs:
- flow block model
- deep work operating system
- focus MOC

#### 1D. Interview / technical prep systems
Suggested files:
- `Interview Prep Guide.md`
- `Master Interview Behavioral Practice Checklist.md`
- `System Design & Technical Prep Checklist.md`
- `DSA_Learning_and_Interview_Principles.md`
- `Feynman_Technique_Study_Method.md`

Likely outputs:
- interview preparation system project
- interview feedback loop model
- reference register

### Phase 2 — NOTES canonicalization

#### 2A. Existing MOCs / dashboard / indexes
Suggested files:
- `MOC - Character Studies.md`
- `MOC - Core Philosophy.md`
- `MOC - Habits & Discipline.md`
- `MOC - Learning & Career.md`
- `MOC - Mindset & Mental Models.md`
- `MOC - Productivity.md`
- `MOC - Systems & Frameworks.md`
- `Vault Dashboard.md`
- `Indexes.md`
- `Home.md`

Goal:
Merge old navigation into canonical `03_MAPS_OF_CONTENT/` structure.

#### 2B. Book summaries
Suggested files:
- `Book Summary - Atomic Habits.md`
- `Book Summary - Deep Work.md`
- `Book Summary - Essentialism.md`
- `Book Summary - Grit.md`
- `Book Summary - The Obstacle Is the Way.md`

Goal:
Preserve as references, selectively extract models/atomic notes.

#### 2C. Technical / career guides
Suggested files:
- `1. Engineering Career Hub (Index).md`
- `Backend Technologies Guide.md`
- `Frontend and Scripting Guide.md`
- `Technical Deep Dives.md`
- `Software Engineering Hub.md`
- `Cloud-Native & DevOps Roadmap.md`

Goal:
Create software engineering MOCs, study projects, and reference registers.

#### 2D. Identity / philosophy / character
Suggested files:
- `Purpose_and_Meaning.md`
- `Discipline_and_Keizoku.md`
- `Character Study - *.md`
- `Subjectivity is cancerous.md`
- `Core Philosophy.md`

Goal:
Route personal/reflection material carefully; extract only durable reusable principles.

### Phase 3 — STUDY_MATERIAL root markdown
Process markdown/project files before binaries.

Focus files:
- learning roadmaps
- LeetCode templates
- system design notes
- career/job search docs
- action plans

Goal:
Create study projects, reference registers, technical MOCs, and reusable protocols.

### Phase 4 — Company-specific packets

Process Doordash before Amazon because it is smaller.

Doordash outputs:
- `Project - Doordash Interview Prep.md`
- `Reference - Doordash Study Register.md`
- `MOC - Company Interview Prep.md`

Amazon outputs:
- `Project - Amazon SDE Interview Prep.md`
- `Reference - Amazon Study Register.md`
- `MOC - Amazon Interview Prep.md`
- leadership principles register
- system design prep register
- LeetCode/problem register

### Phase 5 — Binary/reference indexing
For PDFs/DOCX/ZIP:
1. Create attachment inventory.
2. Identify duplicates.
3. Create companion reference notes.
4. Extract only high-value concepts, models, or protocols.
5. Retain source files by default.

## 8. Quality gates

A batch is not closed until:
- all generated notes have source traceability
- every source has a status
- MOCs/registers are updated
- duplicate/canonical decisions are documented
- unresolved items are tracked
- quality-review-v2 returns PASS or explicit safe-to-proceed

## 9. Anti-patterns

Avoid:
- over-atomicizing lists
- converting every sentence into a note
- forcing models for decoration
- summarizing PDFs without source indexing
- moving/deleting before corrections
- treating journal entries as generic advice
- creating MOCs with too few links or no retrieval value
- processing giant folders without function-based routing

## 10. Default next action

If no other instruction is given, continue from the current open loop:

1. Apply LISTS corrections.
2. Rerun LISTS quality review v2.
3. Apply LISTS retention actions only if safe.
4. Start SYSTEMS habit/routine/time architecture cluster.
