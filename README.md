# ServiceNow Ticket Data Quality Dashboard (Excel + CSV)

A **single-file** HTML dashboard that can read both **Excel (.xlsx / .xls)** and **CSV** files directly in the browser.

## Key Features
- Supports Excel files natively (no conversion needed)
- Also supports CSV
- 100% offline after first load
- No installation, no Node.js, no build step
- All original data quality rules included:
  - Mandatory worknotes (≥15 characters)
  - SLA compliance
  - Completeness + field accuracy
- Full interactive UI: filters, charts, table, modal, export

## How Excel Support Works

This version uses **SheetJS** (loaded via CDN):
- https://cdn.jsdelivr.net/npm/xlsx@0.18.5/dist/xlsx.full.min.js

Once the page loads once, the library is cached and everything works completely offline.

## How to Use

1. Open `index.html` in any modern browser (Chrome, Firefox, Edge)
2. Click **"Upload Excel or CSV"**
3. Or click **"Load Sample Data"** to test immediately
4. Use filters, view charts, click rows for details, and export

## Recommended Excel Columns

Use the same standard ServiceNow fields:

```
number,short_description,description,state,priority,assignment_group,assigned_to,opened_at,closed_at,resolved_at,work_notes,sla_due,made_sla
```

## New GitHub Repo

https://github.com/confusoo/sn-quality-dashboard-excel-html

## Related Project

Original React version: https://github.com/confusoo/sn-ticket-quality-dashboard  
Pure CSV single-file version: https://github.com/confusoo/sn-quality-dashboard-html

## License

MIT
