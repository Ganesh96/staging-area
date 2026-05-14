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
| 2026-05-02 | move-to-holding | 01_STAGING/00_INBOX_DUMP/LISTS/Behavioral_Interview_Links.md | Empty placeholder in LISTS batch | None | no inbound links in generated LISTS outputs | codex-agent | 2026-05-02 | 2026-06-01 | Moved after LISTS v2 review marked retention safe. |
| 2026-05-02 | move-to-holding | 01_STAGING/00_INBOX_DUMP/LISTS/Inbox.md | Empty placeholder in LISTS batch | None | no inbound links in generated LISTS outputs | codex-agent | 2026-05-02 | 2026-06-01 | Moved after LISTS v2 review marked retention safe. |
| 2026-05-02 | move-to-holding | 01_STAGING/00_INBOX_DUMP/LISTS/Resources - CodeCrafters.md.md | Empty placeholder / typo variant placeholder | None | no inbound links in generated LISTS outputs | codex-agent | 2026-05-02 | 2026-06-01 | Moved after LISTS v2 review marked retention safe. |

- 2026-05-14 | moved processed source folders to trash-holding archives:
  - 00_INBOX_DUMP/* -> 99_TRASH_HOLDING/ROOT_00_INBOX_DUMP_2026-05-14/
  - 01_STAGING/00_INBOX_DUMP/* -> 99_TRASH_HOLDING/STAGING_00_INBOX_DUMP_2026-05-14/
  - 01_STAGING/01_LONG_FORM/NOTES/* -> 99_TRASH_HOLDING/STAGING_LONG_FORM_NOTES_2026-05-14/

- 2026-05-14 | moved processed systems sources to trash-holding archive:
  - 01_STAGING/01_LONG_FORM/SYSTEMS/* -> 99_TRASH_HOLDING/STAGING_LONG_FORM_SYSTEMS_2026-05-14/
