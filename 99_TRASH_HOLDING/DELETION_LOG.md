# Deletion Log

Tracks all candidate moves to `99_TRASH_HOLDING/` and all permanent deletions.
No records yet.

## Usage rules
- Every move-to-holding and deletion gets one row.
- Deletion rows must reference prior holding row.
- Never delete without completed safety checks.

## Columns
| Date | Action | File Path | Reason | Canonical Replacement | Link Check | Approved By | Hold Start | Hold End | Notes |
|---|---|---|---|---|---|---|---|---|---|

## Entries
| Date | Action | File Path | Reason | Canonical Replacement | Link Check | Approved By | Hold Start | Hold End | Notes |
|---|---|---|---|---|---|---|---|---|---|
| 2026-05-02 | move-to-holding | 01_STAGING/00_INBOX_DUMP/TEXT/Untitled.md | Empty/placeholder; no retained content required | None | no inbound links found in batch outputs | codex-agent | 2026-05-02 | 2026-06-01 | Retention policy cooldown started; no permanent delete performed. |
| 2026-05-02 | move-to-holding | 01_STAGING/00_INBOX_DUMP/TEXT/a.md | Instruction prompt/meta note, low domain value after extraction review | None | no inbound links found in batch outputs | codex-agent | 2026-05-02 | 2026-06-01 | Hold for 30 days before delete eligibility review. |
