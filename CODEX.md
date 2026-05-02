# CODEX Instructions

This repository is an Obsidian second-brain staging and transformation system.

The objective is not generic cleanup. The objective is to convert messy personal notes, lists, guides, references, projects, journals, PDFs, DOCX files, and study material into a practical, retrieval-first Obsidian vault.

## Core operating rule

- Folder = function
- Link = meaning
- Tag = status or cross-cutting property
- MOC = retrieval path

Use `ARCHITECTURE.md`, `RETENTION_POLICY.md`, `PROCESSING_STRATEGY.md`, `01_STAGING/PROCESSING_AUDIT.md`, and `09_TEMPLATES/` as governing documents.

## Primary objective

Transform raw and staged material into structured, traceable, reusable Obsidian artifacts while preserving source meaning.

Target outputs:
- `02_ATOMIC_NOTES/` — reusable single-idea notes
- `03_MAPS_OF_CONTENT/` — navigation hubs and retrieval paths
- `04_PROJECTS/` — execution systems, active plans, job/interview prep
- `05_REFERENCES/` — source registers, attachment indexes, book/link/PDF/DOCX references
- `06_JOURNAL/` — personal reflection, identity, emotional material
- `07_MODELS/` — reusable frameworks, protocols, lenses, algorithms
- `08_DECISIONS/` — decisions, tradeoffs, forecasts, postmortems
- `09_TEMPLATES/` — canonical templates
- `99_TRASH_HOLDING/` — reversible deletion buffer

## Processing doctrine

Process by function first, folder second.

Before processing any batch, classify each source as one or more:
- raw idea
- list/register
- guide
- checklist
- project/action material
- model/framework
- journal/reflection
- source/reference
- duplicate/variant
- placeholder
- binary attachment

Then choose the transformation:
- raw idea -> atomic note only if reusable
- list/register -> reference register or MOC
- guide -> reference note plus practical checklist/model only if useful
- checklist -> executable protocol
- project/action material -> project note, task system, or decision log
- model/framework -> model note
- journal/reflection -> journal note; protect original meaning
- source/reference -> reference note; preserve original
- duplicate/variant -> canonicalization recommendation with aliases
- placeholder -> needs-review or trash candidate
- binary attachment -> attachment index first; selective extraction later

Do not process all files the same way.

## Batch lifecycle

Every meaningful batch must follow this sequence:

1. Processing
2. Quality review
3. Corrections
4. Quality review v2
5. Retention actions
6. Next batch

Never perform retention actions before quality review and corrections are complete.

## Processing constraints

- Do not delete source files during processing.
- Do not move originals during processing unless the task is explicitly a retention-action task.
- Do not permanently delete anything unless `RETENTION_POLICY.md` deletion gates are satisfied.
- Preserve source traceability through `source_notes`, registers, and batch reports.
- Do not over-atomicize simple lists, inventories, watchlists, or source registers.
- Do not force models where they do not add practical value.
- Do not turn journal or identity material into generic advice.
- Do not summarize PDFs/DOCX/ZIPs as the first pass; create attachment/reference indexes first.
- Do not process new folders during review/correction/retention tasks.

## Cross-folder processing rule

Cross-folder clustering is allowed only when the task explicitly names every source file.

Use cross-folder clusters for obvious duplicates or related concepts, such as:
- routine/time architecture variants
- flow/focus variants
- book/resource duplicates
- interview-prep materials across folders
- company-specific study packets

Do not run broad commands like “process all SYSTEMS and NOTES” unless explicitly requested.

## Retention and deletion

Use `RETENTION_POLICY.md`.

Permanent deletion is allowed only after:
- source has completed the relevant batch lifecycle
- canonical replacement exists or file is confirmed useless noise
- no active backlinks depend on it
- move/deletion is logged in `99_TRASH_HOLDING/DELETION_LOG.md`
- required hold period is satisfied
- file is not protected journal/source/project/governance material

Default action for uncertainty: mark `needs-review`, not delete.

## Current strategic order

1. Close LISTS batch: corrections -> quality-review-v2 -> retention actions.
2. Process SYSTEMS by function-based clusters:
   - habit/routine/time architecture
   - procrastination/habit mechanics
   - flow/focus systems
   - interview/technical prep systems
3. Process NOTES by canonicalization clusters:
   - existing MOCs/dashboard/indexes
   - book summaries
   - technical/career guides
   - identity/philosophy/character notes
4. Process STUDY_MATERIAL markdown and project material.
5. Process Doordash packet before Amazon.
6. Process Amazon markdown/project packet.
7. Create binary attachment indexes for PDFs/DOCX/ZIPs.
8. Extract from PDFs/DOCX only selectively, after indexing.

## Required batch report sections

Each processing report should include:
- source scope
- files processed
- source classification table
- outputs created
- duplicate/variant clusters
- low-value/placeholder candidates
- practical-resource transformations
- MOCs created/updated
- unresolved items
- retention recommendation per source
- recommended next batch

Each quality review should include:
- pass/fail verdict
- priority issue matrix
- file-by-file review
- note-level issues
- missing practical artifacts
- recommended corrections
- retention readiness
- whether the batch is safe to close or proceed
