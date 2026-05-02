# Obsidian Vault Processing Audit

_Date audited: 2026-05-02 (UTC)_

## Coverage summary
Scope audited:
- `00_INBOX_DUMP/`
- `01_STAGING/00_INBOX_DUMP/`
- `01_STAGING/01_LONG_FORM/`
- all nested subfolders

### High-level totals (in audited scope)
- Total files: **248**
- Processed into atomic notes: **12**
- Unprocessed (raw/staging/reference/templates/projects): **236**
- Empty/placeholder files: **11**
- Exact-duplicate content groups: **2 groups**

> Processing status definition used in this audit:
> - **Processed** = files in `01_STAGING/00_INBOX_DUMP/ATOMIC_NOTES/` that are Obsidian-ready atomic notes.
> - **Unprocessed** = everything else (raw inbox, staging lists/text, long-form notes, study material, PDFs/DOCX/ZIP).

---

## Folder-by-folder status

| Folder | Total files | Processed files | Unprocessed files | Empty / placeholders | Notes |
|---|---:|---:|---:|---:|---|
| `00_INBOX_DUMP/` | 6 | 0 | 6 | 3 | Raw inbox sources; includes small plaintext scratch files. |
| `01_STAGING/00_INBOX_DUMP/ATOMIC_NOTES/` | 12 | 12 | 0 | 0 | Fully processed atomic-note output set (current processed corpus). |
| `01_STAGING/00_INBOX_DUMP/JOURNAL/` | 8 | 0 | 8 | 0 | Preserve as journal/templates; not atomicized yet. |
| `01_STAGING/00_INBOX_DUMP/LISTS/` | 47 | 0 | 47 | 3 | Large backlog; multiple overlap/duplication candidates. |
| `01_STAGING/00_INBOX_DUMP/TEMPLATES/` | 1 | 0 | 1 | 0 | Template asset; preserve as canonical template. |
| `01_STAGING/00_INBOX_DUMP/TEXT/` | 10 | 0 | 10 | 0 | Raw text fragments; needs triage + decomposition. |
| `01_STAGING/01_LONG_FORM/` | 1 | 0 | 1 | 0 | Contains `STUDY_MATERIAL.zip` archive. |
| `01_STAGING/01_LONG_FORM/NOTES/` | 51 | 0 | 51 | 3 | Long-form note library with likely overlap variants. |
| `01_STAGING/01_LONG_FORM/STUDY_MATERIAL/` | 31 | 0 | 31 | 1 | Mixed markdown + binaries (pdf/docx). |
| `01_STAGING/01_LONG_FORM/STUDY_MATERIAL/Amazon/` | 29 | 0 | 29 | 1 | Project/reference packet; includes markdown and interview docs. |
| `01_STAGING/01_LONG_FORM/STUDY_MATERIAL/Amazon/pdfs/` | 15 | 0 | 15 | 0 | Binary-heavy reference subset. |
| `01_STAGING/01_LONG_FORM/STUDY_MATERIAL/Doordash/` | 5 | 0 | 5 | 0 | Project/reference packet. |
| `01_STAGING/01_LONG_FORM/SYSTEMS/` | 32 | 0 | 32 | 0 | Systems/process library; many candidates for atomic decomposition. |

---

## File classification table

| Class | Description | Current locations | Count (approx) | Preserve as |
|---|---|---|---:|---|
| Atomic notes (processed) | Obsidian-ready, structured atomic units | `01_STAGING/00_INBOX_DUMP/ATOMIC_NOTES/` | 12 | **Atomic notes** |
| Raw inbox capture | Minimal/rough captures, unnormalized | `00_INBOX_DUMP/`, `01_STAGING/00_INBOX_DUMP/TEXT/` | 16 | **Raw capture / backlog** |
| Lists and resource collections | Curated or semi-curated lists | `01_STAGING/00_INBOX_DUMP/LISTS/` | 47 | **Reference or project notes** |
| Journal/review templates & personal reflections | Review cadence + identity notes | `01_STAGING/00_INBOX_DUMP/JOURNAL/` | 8 | **Journal notes** |
| Templates | Reusable note structures | `01_STAGING/00_INBOX_DUMP/TEMPLATES/`, long-form templates | 3+ | **Templates** |
| Long-form conceptual notes | Essays, guides, hubs, MoCs | `01_STAGING/01_LONG_FORM/NOTES/`, `SYSTEMS/` | 83 | **Long-form reference / model / systems notes** |
| Project-specific study packs | Interview/company prep artifacts | `01_STAGING/01_LONG_FORM/STUDY_MATERIAL/` (+ `Amazon`, `Doordash`) | 80 | **Project/reference notes** |
| Binary reference assets | PDFs, DOCX, ZIP | `01_STAGING/01_LONG_FORM/**` | 40+ | **Reference attachments** |

---

## Empty/placeholder files

### Confirmed empty or whitespace-only
- `00_INBOX_DUMP/.gitkeep`
- `00_INBOX_DUMP/job sites`
- `00_INBOX_DUMP/sticknote_password`
- `01_STAGING/00_INBOX_DUMP/LISTS/Behavioral_Interview_Links.md`
- `01_STAGING/00_INBOX_DUMP/LISTS/Inbox.md`
- `01_STAGING/00_INBOX_DUMP/LISTS/Resources - CodeCrafters.md.md`
- `01_STAGING/01_LONG_FORM/NOTES/3. Technical Deep Dives.md`
- `01_STAGING/01_LONG_FORM/NOTES/Core Philosophy.md`
- `01_STAGING/01_LONG_FORM/NOTES/Home.md`
- `01_STAGING/01_LONG_FORM/STUDY_MATERIAL/Recommendation Engine Design.md`
- `01_STAGING/01_LONG_FORM/STUDY_MATERIAL/Amazon/LPs.md`

---

## Duplicate / near-duplicate candidates

### Exact duplicate content (hash-identical)
1) **Empty-file group** (all zero-byte/blank):
- `00_INBOX_DUMP/.gitkeep`
- `00_INBOX_DUMP/job sites`
- `01_STAGING/00_INBOX_DUMP/LISTS/Inbox.md`
- `01_STAGING/00_INBOX_DUMP/LISTS/Behavioral_Interview_Links.md`
- `01_STAGING/00_INBOX_DUMP/LISTS/Resources - CodeCrafters.md.md`
- `01_STAGING/01_LONG_FORM/NOTES/3. Technical Deep Dives.md`
- `01_STAGING/01_LONG_FORM/NOTES/Home.md`
- `01_STAGING/01_LONG_FORM/NOTES/Core Philosophy.md`
- `01_STAGING/01_LONG_FORM/STUDY_MATERIAL/Recommendation Engine Design.md`
- `01_STAGING/01_LONG_FORM/STUDY_MATERIAL/Amazon/LPs.md`

2) **Binary duplicate**:
- `01_STAGING/01_LONG_FORM/STUDY_MATERIAL/Amazon/Medium - Behavioral Interview Questions.pdf`
- `01_STAGING/01_LONG_FORM/STUDY_MATERIAL/Amazon/pdfs/Medium - Behavioral Interview Questions.pdf`

### Near-duplicate filename/topic candidates (manual review needed)
- `Books.md` vs `Booksss.md` vs `Books - Progress.md`
- `Resources - Websites.md` vs `Resources - Websitesss.md`
- `Flow State.md` vs `Flow_State.md`
- `How to Create a Routine.md` appears in both `NOTES/` context and `SYSTEMS/` (and prefixed variant `1. How to Create a Routine.md`)
- `K Step for Flow.md` vs `K-Step Guide to Flow.md`
- `Technical Deep Dives.md` vs `3. Technical Deep Dives.md`
- `Character Study - Kangiten.md` vs `Character Study - Kangitenn.md`
- `Character Study - Count Alexander Ilyich Rostov.md` vs `Character Study - Count Ilyich Rostov.md`

---

## Unprocessed backlog

### Backlog by likely processing mode
1. **Atomic extraction candidates (highest value, markdown, action-oriented):**
   - `01_STAGING/00_INBOX_DUMP/LISTS/*.md`
   - `01_STAGING/00_INBOX_DUMP/TEXT/*.md`
2. **System/model decomposition candidates:**
   - `01_STAGING/01_LONG_FORM/SYSTEMS/*.md`
   - selected `01_STAGING/01_LONG_FORM/NOTES/*.md`
3. **Project/reference packet normalization (company-specific):**
   - `01_STAGING/01_LONG_FORM/STUDY_MATERIAL/Amazon/*.md`
   - `01_STAGING/01_LONG_FORM/STUDY_MATERIAL/Doordash/*.md`
4. **Attachment indexing only (not full decomposition first pass):**
   - PDFs / DOCX / ZIP under `01_STAGING/01_LONG_FORM/STUDY_MATERIAL/**`

---

## Recommended next processing order

1. **Batch 2A: `01_STAGING/00_INBOX_DUMP/LISTS/` (priority)**
   - Convert list-style notes into atomic decisions/tasks/resources.
   - Resolve duplicates and typo-variants into canonical note IDs (without deleting originals yet).

2. **Batch 2B: `01_STAGING/00_INBOX_DUMP/TEXT/`**
   - Triage fragments (`Untitled*`, single-letter files) into either atomic notes or archive/open-loop notes.

3. **Batch 3: `01_STAGING/01_LONG_FORM/SYSTEMS/`**
   - Decompose process frameworks into reusable models, checklists, and protocols.

4. **Batch 4: `01_STAGING/01_LONG_FORM/NOTES/`**
   - Start with MoCs/hubs and obvious near-duplicates, then decompose concept notes.

5. **Batch 5: `01_STAGING/01_LONG_FORM/STUDY_MATERIAL/**`**
   - Markdown first, then build attachment index notes for binaries (PDF/DOCX/ZIP).

---

## Risks or ambiguities

- **Processed-definition ambiguity:** only `ATOMIC_NOTES/` is clearly processed; some long-form notes may already be semi-structured but not atomic.
- **Binary-heavy folders:** PDFs/DOCX/ZIP cannot be fully audited semantically without extraction/parsing.
- **Naming noise:** typo/variant names make canonical linking brittle (`Booksss`, `Websitesss`, `Kangitenn`, etc.).
- **Empty placeholders:** multiple empty files can create false backlog volume and confusion about intent.
- **Cross-folder overlap:** similar topics split across `LISTS`, `NOTES`, `SYSTEMS`, and `STUDY_MATERIAL` may require a canonical source-of-truth strategy before merge/reorg.
