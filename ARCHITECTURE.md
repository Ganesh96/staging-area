# Obsidian Second-Brain Architecture (Target Design)

Context source: `01_STAGING/PROCESSING_AUDIT.md`.

## 1) Core operating rule
- **Folder = function**
- **Link = meaning**
- **Tag = status or cross-cutting property**
- **MOC = retrieval path**

This architecture is retrieval-first, durable Markdown-first, and staged for safe incremental migration.

---

## 2) Folder structure and purpose

- `00_INBOX_DUMP/` — raw capture only. No structure pressure.
- `01_STAGING/` — temporary processing workspace, audits, batch reports.
- `02_ATOMIC_NOTES/` — one reusable idea per note (evergreen candidates).
- `03_MAPS_OF_CONTENT/` — topic hubs, indexes, reading paths.
- `04_PROJECTS/` — active execution artifacts (plans, trackers, outcomes).
- `05_REFERENCES/` — source notes and preserved material (books, links, PDFs, DOCX metadata notes).
- `06_JOURNAL/` — reflections, identity processing, periodic reviews.
- `07_MODELS/` — reusable models/frameworks/lenses.
- `08_DECISIONS/` — decision records, tradeoffs, forecasts, postmortems.
- `09_TEMPLATES/` — canonical note templates.
- `99_TRASH_HOLDING/` — reversible deletion buffer.

---

## 3) Note types and where they live

- **Atomic note** → `02_ATOMIC_NOTES/`
- **MOC** → `03_MAPS_OF_CONTENT/`
- **Project note** → `04_PROJECTS/`
- **Reference note** → `05_REFERENCES/`
- **Journal note** → `06_JOURNAL/`
- **Model note** → `07_MODELS/`
- **Decision log** → `08_DECISIONS/`
- **Processing report/audit** → `01_STAGING/`

---

## 4) Naming conventions

- Atomic notes: `Concept - Specific Claim.md` (e.g., `Attention - Single-Threading Reduces Context Loss.md`)
- MOCs: `MOC - Topic.md`
- Models: `Model - Name.md`
- Projects: `Project - Name.md`
- Decisions: `Decision - YYYY-MM-DD - Topic.md`
- Journal: `Journal - YYYY-MM-DD.md`
- Reference notes: `Reference - Source - Topic.md`

Rules:
- Keep names human-scannable and stable.
- Use singular canonical names; avoid typo-variants.
- Add `aliases` in frontmatter instead of duplicate notes.

---

## 5) Tag conventions

Use tags for **status and cross-cutting properties**, not primary taxonomy.

### Status tags
- `#status/raw`
- `#status/staged`
- `#status/processed`
- `#status/evergreen`
- `#status/reference`
- `#status/project-active`
- `#status/archived`
- `#status/needs-review`
- `#status/duplicate-candidate`
- `#status/empty-placeholder`

### Cross-cutting tags
- Domain: `#domain/learning`, `#domain/job-search`, `#domain/systems`
- Note type (optional): `#type/atomic`, `#type/model`, `#type/moc`
- Quality: `#quality/source-backed`, `#quality/draft`

---

## 6) Backlink conventions

- Every atomic note should link to at least one MOC.
- Every project note links to supporting atomic/model/decision notes.
- Reference notes should link **from source → extracted insights**.
- Use explicit relation language in body:
  - “Connects to [[...]] because …”
  - “Contrasts with [[...]]”
  - “Depends on [[...]]”

---

## 7) Creation rules (decision criteria)

### Create an atomic note when
- A single idea is reusable across contexts.
- The note can stand alone without source re-reading.
- It expresses one claim/insight/heuristic/definition.

### Create a model note when
- A framework can be repeatedly applied to decisions or analysis.
- Multiple notes can be interpreted via the same lens.

### Create a MOC when
- A topic has 7+ related notes OR retrieval feels slow.
- You need a guided entry point for future you.

### Keep as reference when
- Content is source-preservation, not distilled knowledge.
- Binary attachments (PDF/DOCX/ZIP) or verbatim source excerpts.

### Keep as journal when
- The value is temporal/personal reflection, not generalizable claim.

### Keep as project/action when
- The note tracks outcomes, tasks, milestones, constraints, execution logs.

---

## 8) Special handling rules

### Duplicates
- Never delete immediately.
- Mark both with `#status/duplicate-candidate`.
- Create/choose canonical note; add aliases and redirect links.
- Move deprecated duplicate to `99_TRASH_HOLDING/` only after link migration.

### Empty/placeholder files
- Mark `#status/empty-placeholder`.
- Add one-line intent + next action + review date.
- If no intent after two review cycles, archive candidate.

### Uncertain notes
- Route to `01_STAGING/` with `#status/needs-review`.
- Add “uncertainty question” and minimum disambiguation steps.

### PDFs/DOCX/source material
- Preserve originals in `05_REFERENCES/attachments/` (or existing source location until migration).
- Create companion reference note per source with metadata + extracted claims.
- Do not copy large excerpts; link and paraphrase.

### Future inbox additions
- All new captures enter `00_INBOX_DUMP/`.
- Weekly processing batch: inbox → staging triage → destination notes.
- No direct write to atomic/model folders without staging pass.

---

## 9) Minimal frontmatter schemas

### Atomic
```yaml
id: atomic-YYYYMMDD-slug
type: atomic
status: processed
created: YYYY-MM-DD
updated: YYYY-MM-DD
tags: []
aliases: []
source_notes: []
moc: []
```

### Model
```yaml
id: model-YYYYMMDD-slug
type: model
status: evergreen
created: YYYY-MM-DD
updated: YYYY-MM-DD
tags: []
aliases: []
applicable_domains: []
related_models: []
```

### MOC
```yaml
id: moc-YYYYMMDD-topic
type: moc
status: evergreen
created: YYYY-MM-DD
updated: YYYY-MM-DD
tags: []
scope: topic
```

### Project
```yaml
id: project-YYYYMMDD-slug
type: project
status: project-active
created: YYYY-MM-DD
updated: YYYY-MM-DD
owner: self
goal: ""
review_cadence: weekly
```

### Decision
```yaml
id: decision-YYYYMMDD-topic
type: decision
status: processed
created: YYYY-MM-DD
updated: YYYY-MM-DD
decision_date: YYYY-MM-DD
context: ""
```

### Reference
```yaml
id: ref-YYYYMMDD-slug
type: reference
status: reference
created: YYYY-MM-DD
updated: YYYY-MM-DD
source_type: [book|pdf|article|video|docx|web]
source_link: ""
```

### Journal
```yaml
id: journal-YYYYMMDD
type: journal
status: archived
created: YYYY-MM-DD
updated: YYYY-MM-DD
mood: ""
```

---

## 10) Migration strategy (no file moves yet; execution plan)

1. Freeze architecture and templates (this deliverable).
2. Use `01_STAGING/PROCESSING_AUDIT.md` as backlog ledger.
3. Process in batches; create new canonical notes in target folders.
4. Add aliases/redirect links for duplicate candidates.
5. After link stabilization, move deprecated items to `99_TRASH_HOLDING/`.
6. Run monthly retrieval QA (broken links, orphan notes, stale statuses).

---

## 11) First 5 MOCs to create

1. `MOC - Job Search Execution`
2. `MOC - Learning Systems`
3. `MOC - Interview Preparation`
4. `MOC - Attention and Productivity`
5. `MOC - Personal Operating System`

---

## 12) Recommended processing order (from current audit)

1. `01_STAGING/00_INBOX_DUMP/LISTS/` (highest actionable backlog)
2. `01_STAGING/00_INBOX_DUMP/TEXT/` (fragment triage)
3. `01_STAGING/01_LONG_FORM/SYSTEMS/` (framework decomposition)
4. `01_STAGING/01_LONG_FORM/NOTES/` (dedupe + atomic extraction)
5. `01_STAGING/01_LONG_FORM/STUDY_MATERIAL/**` (reference indexing first)

---

## 13) Quality-control checklist (per processing batch)

- [ ] Source file preserved unchanged.
- [ ] Each new atomic note has one idea only.
- [ ] Frontmatter complete and valid.
- [ ] At least one MOC link added.
- [ ] Status tag assigned.
- [ ] Duplicate check performed.
- [ ] Empty placeholders explicitly marked.
- [ ] Next-action backlog updated.

---

## 14) Guardrails

### Prevent over-fragmentation
- Do not split unless each child note is independently reusable.
- Minimum threshold: a split must add a new retrievable claim.
- Keep tightly coupled steps together in one protocol note.

### Prevent bloated notes
- If a note has >3 distinct claims, split into atomic children.
- If a note mixes source dump + interpretation + tasks, separate by type.
- Keep project notes execution-focused; move theory to atomic/model notes.
