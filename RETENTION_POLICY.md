# Vault Retention Policy

Sources used:
- `ARCHITECTURE.md`
- `01_STAGING/PROCESSING_AUDIT.md`

This policy defines when files are preserved, marked for review, moved to `99_TRASH_HOLDING/`, or permanently deleted.

## 1) Retention classes

### A. Preserve permanently
Keep indefinitely when any of the following is true:
1. Note is a canonical atomic, model, MOC, decision, project, reference, or journal note with active backlinks.
2. Note is a source artifact (PDF/DOCX/ZIP/book/article export) with ongoing reference value.
3. Note is a processing artifact needed for governance/history (audit reports, batch reports, architecture rules, templates).
4. Note has non-recoverable personal reflection value (journal/reflection/identity content).

### B. Mark `needs-review`
Apply when any of the following is true:
1. Intent is unclear or note is ambiguous.
2. Note is likely duplicate but canonical version is not confirmed.
3. Note is empty/placeholder but expected to be filled.
4. Note contains partial extraction from source material with unresolved follow-up.

### C. Move to `99_TRASH_HOLDING/`
Use reversible holding when file is not currently needed but deletion is not yet safe:
1. Duplicate confirmed and canonical successor exists.
2. Placeholder/empty note is stale (fails review criteria below).
3. Deprecated working files replaced by canonical notes.
4. Temporary exports/intermediate artifacts no longer required but potentially recoverable.

### D. Permanently delete
Allowed only after strict conditions + safety checks pass.

---

## 2) Strict deletion conditions (all mandatory)

A file can be permanently deleted only if **all** conditions are met:
1. It has spent at least one full review cycle in `99_TRASH_HOLDING/`.
2. Canonical replacement exists (or file is confirmed useless noise).
3. No inbound links remain from active notes.
4. Entry exists in `99_TRASH_HOLDING/DELETION_LOG.md` with rationale.
5. File is not a protected class (journal, source attachments, architecture/policy/template, active project material).
6. A maintainer verifies recoverability or irrelevance.

If any condition fails: do not delete.

---

## 3) Safety checks before deletion

Run this checklist before deleting anything:
- [ ] Backlink check: no active notes depend on it.
- [ ] Canonical check: replacement note exists and is linked.
- [ ] Source check: not original-only source material.
- [ ] Journal check: not personal reflection content.
- [ ] Decision/history check: not needed for audit trail.
- [ ] Log check: move/deletion recorded in `DELETION_LOG.md`.
- [ ] Cooldown check: elapsed hold period completed.

Recommended minimum hold period:
- Low-risk duplicates/placeholders: 30 days
- High-risk materials (project/source/history): 90 days+

---

## 4) Duplicate handling policy

1. Mark candidates with `#status/duplicate-candidate`.
2. Choose a canonical note by:
   - clearer title
   - richer content quality
   - stronger backlink connectivity
   - better schema/template compliance
3. Add aliases to canonical note for known variants.
4. Update/redirect links from duplicates to canonical note.
5. Move non-canonical duplicates to `99_TRASH_HOLDING/` (not immediate deletion).
6. Delete only after hold period and safety checks.

Special case from audit:
- Exact duplicate binary files (same hash) should keep one canonical copy plus one reversible candidate in holding until links/usages are verified.

---

## 5) Empty/placeholder file policy

### Classification
- **Intentional placeholders**: valid if they include explicit next step + review date.
- **Unintentional empties**: noise by default.

### Workflow
1. Mark empty files `#status/empty-placeholder` (or in tracking notes when file has no frontmatter).
2. Add intent statement and deadline where possible.
3. If untouched for two review cycles:
   - move to `99_TRASH_HOLDING/`
4. If still unused after hold period and no links:
   - eligible for permanent deletion.

Do not delete `.gitkeep` files if they are required to preserve directory structure.

---

## 6) Journal retention policy

Journal and reflection content is protected by default.

Rules:
1. Never permanently delete journal notes during normal cleanup.
2. Do not move active journal notes to trash holding.
3. If redaction is needed (privacy/security), archive secured copy before changes.
4. Journal entries may be summarized into atomic insights, but originals remain preserved.

---

## 7) PDFs, DOCX, ZIP, and reference material policy

1. Preserve original source files by default.
2. Prefer companion reference notes for extracted claims instead of modifying original binaries.
3. Delete only when all are true:
   - exact duplicate confirmed,
   - canonical source retained,
   - no active references/links,
   - hold period + log + safety checks complete.
4. Never delete sole copy of externally sourced research material.

---

## 8) Needs-review routing policy

Send to `needs-review` when uncertain.

Triggers:
- ambiguous title/content
- mixed note types in one file
- unresolved duplicate conflict
- unclear ownership/domain
- security-sensitive placeholders

Required metadata in review note/report:
- why uncertain
- what decision is needed
- deadline for resolution
- owner/reviewer

---

## 9) Operational cadence

- Weekly: review new placeholders, duplicates, and uncertain notes.
- Monthly: review `99_TRASH_HOLDING/` candidates against hold periods.
- Quarterly: prune only items that pass strict deletion conditions.

---

## 10) Non-destructive constraint (current phase)

Current phase explicitly forbids moving/deleting files automatically.
This policy is definitional and preparatory only until a separate execution step is approved.
