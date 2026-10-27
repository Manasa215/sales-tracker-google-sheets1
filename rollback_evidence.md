# Rollback Evidence and Recovery Procedure

## Purpose
Document how to protect the sales tracker before changes and restore a known-good version if formulas or validation rules are damaged.

## Before editing or publishing a new version
1. In Google Drive, make a copy of the workbook with a date in the filename, for example `Sales_Tracker_Backup_2026-10-27`.
2. Confirm the `Raw Sales` and `Summary` tabs exist.
3. Record the current daily/monthly totals and capture a screenshot of the Summary tab.
4. Make changes in a separate copy first.

## Rollback procedure
1. Open the Google Sheets file.
2. Select **File → Version history → See version history**.
3. Select the version immediately before the unwanted change.
4. Review the timestamp and preview, then select **Restore this version** if it is the correct version.
5. Recheck a known daily total, the October monthly total, the Sales Amount formulas, and dropdown validations.

## Evidence to add after you perform the steps
Save screenshots in this folder:
- `evidence/summary_before_change.png`
- `evidence/version_history.png`
- `evidence/summary_after_restore.png`

## Status / honesty note
This repository includes the rollback procedure, not proof that a live Google Sheets rollback has already been performed. Add the screenshots only after performing the steps. Do not represent the template as deployed or rolled back until you have completed and verified those actions.
