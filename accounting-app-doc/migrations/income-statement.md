---
tags: db-view
---
### view *income-statement*

Columns:
- categoryName
- categoryType
- SUM entryValue GROUPED BY categoryID BETWEEN initialDate AND endDate

TABLES:
[[migrations/entries]]
[[categories]]


- categoryID
- categoryName
- categoryType

		category: "revenue",
		label: "Sales",
		value: 100000.00