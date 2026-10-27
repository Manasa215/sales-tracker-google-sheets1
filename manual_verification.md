# Manual Verification of Sample Data

## Independent check
The sample contains 20 orders. For each order, Sales Amount is Units × Unit Price.

- Gross sales across all entered statuses: ₹25,010.00
- Completed-status sales: ₹24,530.00
- Order count: 20

## How to reproduce
1. In `Raw Sales`, multiply Units (column F) by Unit Price (column G) for each populated order.
2. Add the 20 line totals. The independent result is ₹25,010.00.
3. Add only rows whose Status is `Completed`. The independent result is ₹24,530.00.
4. Compare these values with the October 2026 monthly summary after opening the workbook in Google Sheets.

## Note
The returned order is included in gross sales because this example reports the value entered on the order row. The Completed Sales measure excludes `Returned` and `Pending` statuses. For a real business process, define whether returns should be subtracted from net sales and implement that policy consistently.
