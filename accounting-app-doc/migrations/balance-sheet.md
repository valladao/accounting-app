---
tags: db-view
---
### view *balance-sheet*

Columns:
- accountName
- SUM entryValue GROUPED BY accountID UNTIL entryDate
- accountType

TABLES:
[[entries]]
[[accounts]]