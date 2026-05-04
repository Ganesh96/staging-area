---
id: batch-20260504-amazon-quality-gap-review
type: quality-review
status: needs-fix
created: 2026-05-04
updated: 2026-05-04
batch_scope: "Amazon interview-prep deep-processing quality and gap review"
tags: [#ops/quality-review, #ops/needs-fix]
source_notes:
  - 01_STAGING/BATCH_REPORTS/STUDY_MATERIAL-amazon-deep-processing.md
  - 04_PROJECTS/Project - Amazon SDE Interview Preparation.md
  - 03_MAPS_OF_CONTENT/MOC - Amazon Interview Preparation.md
  - 05_REFERENCES/Reference - Amazon Interview Prep Source Register.md
  - 05_REFERENCES/Reference - Amazon Technical Prep Topics Register.md
  - 07_MODELS/Model - Amazon Interview Preparation Stack.md
  - 07_MODELS/Model - Amazon Leadership Principles Behavioral Mapping.md
  - 02_ATOMIC_NOTES/Behavioral - STAR Stories Need Evidence Density to Score Well.md
  - 02_ATOMIC_NOTES/Interview Prep - Company Prep Must Separate Process Patterns and Execution.md
  - 02_ATOMIC_NOTES/System Design - Tradeoff Articulation Matters More Than Component Listing.md
---

# STUDY_MATERIAL Amazon Quality + Gap Review

## Status
**NEEDS_FIX** before moving to next `STUDY_MATERIAL` batch.

Rationale: structural traceability is mostly present, but unresolved high-value PDFs and role-calibration gaps create coverage risk.

---

## 1) Traceability check (source -> outputs)
**Result: PASS (with one caveat).**

- All 9 created Amazon outputs listed in deep-processing report are present.
- All reviewed outputs include `source_notes` frontmatter.
- Source register provides per-file status/triage and downstream mapping.

**Caveat:** one atomic note depends partly on an unreadable PDF source (`Amazon Systems Design Preparation.pdf`), so the source is referenced but not fully validated for extraction fidelity.

---

## 2) Mutual linking check (project/models/MOC/references)
**Result: PASS (minor asymmetry).**

- Project links to MOC + both models + both reference registers.
- MOC links project + models + registers + related systems.
- Both models link to project and MOC.
- Technical register links to project and MOC.

**Minor asymmetry:** source register has no backlinks section. Not required for this pass, but adding links would improve navigation.

---

## 3) Markdown/DOCX over-reliance vs unresolved PDFs
**Result: NEEDS_FIX.**

Deep-processing output quality is driven primarily by readable MD/DOCX sources. Multiple potentially high-value Amazon PDFs remain `unreadable`/`needs-review`, including role-calibration and loop-guidance materials.

Risk: synthesis may be directionally correct but incomplete on loop-specific expectations (especially SDE I vs SDE II phone/onsite calibration).

---

## 4) Unreadable / high-value PDF gap list (priority shortlist)
**Likely highest-value for a PDF-specific pass:**

1. `SDE+II+Phone+Screen+Prep+Guide.pdf` (role-level calibration, likely critical)
2. `SDE Onsite Competency Prep Guide.pdf` (onsite competency rubric)
3. `Candidate Phone Interview Prep.pdf` (screen format + expectations)
4. `Amazon Systems Design Preparation.pdf` (directly referenced in system-design atomic)
5. `STAR Leadership Principals.pdf` (LP-specific behavioral calibration)
6. `Fortify-Experts-Behavioral-Questions-Based-on-Amazon-Principles.pdf` (question bank quality/coverage)
7. `Amazon SDE Interview Prep.pdf` and `Amazon SDE prep.pdf` (possible consolidated playbooks)
8. `SDE Interview Prep Guide 1.pdf` / `2.pdf` / `3.pdf` (multi-part guide set)
9. `pdfs/12 Week Programme - Leetcode.pdf` and `pdfs/Leetcode Quick.pdf` (coding plan acceleration)

**Recommended handling:** run dedicated PDF extraction/triage pass only for the above list; defer low-signal or duplicate PDFs.

---

## 5) Duplicate-note check (new atomics vs existing interview-prep atomics)
**Result: NEEDS_FIX (semantic overlap, not exact duplicates).**

- `Behavioral - STAR Stories Need Evidence Density to Score Well` overlaps with existing `Interviewing - STAR Response Structure Increases Signal`.
- `System Design - Tradeoff Articulation Matters More Than Component Listing` overlaps with existing design-tradeoff interview guidance patterns.
- `Interview Prep - Company Prep Must Separate Process Patterns and Execution` is distinct but adjacent to existing execution-framework notes.

**Action:** mark overlap explicitly in each Amazon atomic with “related/contrast” links (trivial fix) or merge if near-duplicate after PDF pass.

---

## 6) Separation quality: LP, STAR, technical prep, system design
**Result: PASS.**

Current structure separates concerns cleanly:
- LP/behavioral mapping model
- STAR evidence-density atomic
- technical topics register
- system design tradeoff atomic/model linkage

No major category-collision found in scoped files.

---

## 7) SDE I vs SDE II calibration
**Result: NEEDS_FIX.**

Signals exist (e.g., `SDE2 PS prep document -2023.docx` as source), but explicit role split criteria are not codified in scoped artifacts.

Missing explicitness:
- expected depth by round (SDE I vs SDE II)
- system-design bar differences
- behavioral ownership/impact bar differences
- coding expectation delta (speed vs abstraction depth)

---

## 8) SQL-heavy items and role dependence
**Result: NEEDS_FIX (light).**

No explicit SQL calibration note in scoped Amazon artifacts. SQL-heavy prep appears implicitly possible via generic technical materials, but not labeled role-dependent.

Recommended annotation (in technical register/project open loops):
- SQL is role-dependent and team-dependent at Amazon.
- Tag SQL prep as **conditional** unless target org/role interview loop confirms SQL emphasis.

---

## 9) Broken wikilinks / unresolved filenames
**Result: PASS.**

- Scoped files contain no broken wikilinks from static existence check.
- Filename references in source registers resolve as written for scoped dataset.

---

## 10) YAML/frontmatter validity and parseability
**Result: NEEDS_FIX (verification tooling gap, not obvious syntax defect).**

- Frontmatter blocks are consistently present and structurally similar.
- Full YAML parse validation could not be executed in this environment because `pyyaml` is unavailable.

No obvious malformed frontmatter was found via manual inspection, but parser-backed validation remains pending.

---

## Corrections needed (targeted, no global interlinking)
1. Add explicit overlap links from Amazon STAR/system-design atomics to existing interviewing atomics to prevent drift.
2. Add explicit SDE I vs SDE II calibration section in Amazon project (or model) with round-by-round depth assumptions.
3. Add SQL role-dependence note in Amazon technical topics register.
4. Run PDF-specific pass on high-priority unreadable list and update source register statuses (`needs-review` -> `processed`/`deferred`) with evidence.
5. Perform parser-backed YAML validation when YAML tooling is available.

---

## Recommended next action
**Do not start next `STUDY_MATERIAL` batch yet.**

Run a focused **Amazon PDF resolution mini-batch** (high-priority shortlist only), then apply minimal corrections above. Re-run this quality review as `v2` and move forward only if unreadable high-value items are resolved or explicitly deferred with rationale.
