# Batch Lifecycle

This file is the mandatory lifecycle contract for all future Codex batch work.

## Core rule

Every substantial processing batch must follow this sequence:

1. Processing
2. Quality review
3. Corrections
4. Quality review v2
5. Retention actions
6. Next batch

Do not skip steps.

## Step definitions

### 1. Processing
Transform the selected source files into architecture-aligned outputs.

Allowed:
- create atomic notes
- create MOCs
- create project notes
- create reference registers
- create journal/model/decision notes
- create processing report

Not allowed:
- move originals
- delete files
- start cleanup

Required output:
`01_STAGING/BATCH_REPORTS/[BATCH]-processing.md`

### 2. Quality review
Review the generated outputs before changing them further.

Allowed:
- create review report
- identify issues
- recommend corrections
- assess retention readiness

Not allowed:
- modify generated notes
- move originals
- delete files

Required output:
`01_STAGING/BATCH_REPORTS/[BATCH]-quality-review.md`

### 3. Corrections
Apply only the fixes identified by the quality review.

Allowed:
- fix traceability
- improve MOC links
- improve registers
- merge/split generated notes
- improve practical usefulness
- create corrections report

Not allowed:
- process new folders
- move originals
- delete files
- expand scope beyond the reviewed batch

Required output:
`01_STAGING/BATCH_REPORTS/[BATCH]-corrections.md`

### 4. Quality review v2
Rerun review after corrections.

Allowed:
- verify corrections
- decide pass/fail
- decide safe-to-proceed
- decide retention readiness

Not allowed:
- modify files
- move originals
- delete files

Required output:
`01_STAGING/BATCH_REPORTS/[BATCH]-quality-review-v2.md`

### 5. Retention actions
Run only if quality-review-v2 explicitly says retention is safe.

Allowed:
- move safe candidates to `99_TRASH_HOLDING/`
- update `99_TRASH_HOLDING/DELETION_LOG.md`
- create retention report

Not allowed:
- permanent deletion unless `RETENTION_POLICY.md` gates are fully satisfied
- touching files outside the batch scope

Required output:
`01_STAGING/BATCH_REPORTS/[BATCH]-retention-actions.md`

### 6. Next batch
Start only after the prior batch is closed or explicitly paused with blockers documented.

## Stop conditions

Stop and report blockers if:
- source traceability is incomplete
- duplicate/canonical decisions are unresolved
- MOC/register linkage is weak
- generated notes are not practically useful
- quality-review-v2 is not PASS or safe-to-proceed
- retention safety is unclear

## Default instruction

If a user says “process this batch,” Codex should automatically interpret that as:

Process only step 1, create the processing report, and stop.

If a user says “close this batch,” Codex should run the remaining lifecycle steps in order, stopping if any gate fails.
