# Departmental Toolkit (prototype v2)

An Excel workbook that tracks document-control logs across five departments in one place. Prototype with dummy data. Rows marked EXAMPLE are fake: delete them and add your own.

By Hussein Abdallah, Document Control.

## What it has
- 11 logs: Technical Office (Technical Submittal, Shop Drawings, RFI, MS), Quality (IR, MIR, TRF, NCR), Safety (Safety Obs), Finance (Payment App, dummy amounts), Admin (Letters).
- Each log calculates Reply Due, Days Waiting and a status (Open / OVERDUE / Closed).
- Related Ref column links a record to a record in another log, with a check that shows NOT FOUND for broken links.
- All Overdue tab: every overdue item from all logs in one list (first 100 shown, total counted in full).
- Safety Training tab: training and certificate expiry with EXPIRED, EXPIRING, Valid, NO EXPIRY and CHECK DATES statuses. The warning period (30 days) is set on Settings.
- Dashboard with totals per log and per department.

## Checked
Results were compared with an independent Python calculation on the example rows, an empty workbook, edge cases and a 110-overdue-item case. Checked in LibreOffice only.

## Limits
- Not tested in desktop Excel or on Windows.
- Department names, columns, statuses and reply periods are placeholders, not any company's procedure. The meaning of IR, MIR, MS, RFI and NCR is assumed.
- All Overdue shows the first 100 items and uses INDIRECT, which recalculates often.
- Safety Training is not linked to the other logs.
- No workflow, approvals or real finance logic. It is a tracker, not a system.
- The name mark is floating pictures over the sheets.

Dummy data only. No employer data.

(c) 2026 Hussein Abdallah, rights reserved.
