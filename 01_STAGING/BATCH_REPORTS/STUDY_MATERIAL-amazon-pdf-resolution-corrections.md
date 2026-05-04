---
id: batch-20260504-amazon-pdf-resolution-corrections
type: corrections
status: processed
created: 2026-05-04
updated: 2026-05-04
batch_scope: "Amazon high-priority PDF resolution + blocker corrections"
tags: [#ops/corrections, #ops/pdf-resolution]
---

# STUDY_MATERIAL Amazon PDF Resolution Corrections

## Methods attempted
- CLI extraction tools: `pdftotext`, `pdfinfo`.
- Python libraries: `pypdf`, `PyPDF2`, `pdfminer`, `fitz/pymupdf`.
- File-level fingerprinting: SHA-256 + size check for shortlist PDFs.

## Environment outcome
- No reliable PDF extraction tooling available in this environment.
- Therefore, high-priority PDFs cannot be marked `processed` without guessing.
- All shortlist PDFs were reclassified to `needs-manual-review` with explicit rationale in source register.

## Shortlist resolution summary
- Processed: 0
- Duplicate (confirmed by hash): 0 within shortlist
- Low-signal: 0
- Unreadable/needs-manual-review: 13

## Additional blocker corrections completed
1. Added explicit SDE I vs SDE II calibration section in Amazon project note.
2. Added SQL role-dependence guidance in technical topics register (conditional lane).
3. Added overlap/related links in the three Amazon atomic notes to reduce drift.
4. Re-ran scoped broken-wikilink existence check (no broken links found).
5. Attempted parser-backed YAML check; parser dependency unavailable (`pyyaml` missing), recorded as pending.

## Deferred items (explicit)
- PDF text extraction/content synthesis for the 13 high-priority PDFs must be completed in an environment with reliable PDF extraction or OCR support.
