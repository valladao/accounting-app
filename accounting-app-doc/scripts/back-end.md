---
tags: architecture script
---

Access [[database]]

### endpoint get(/balance-sheet)

From: [[migrations/balance-sheet]]

Export JSON: *balanceSheet*
```js
{
	[
		account: "Cash",
		total: XX.XX,
		type: "assets"
	],
	[
		account: "Accounts Payable",
		total: XX.XX
		type: "liabilities"
	],
	[
		account: "Earnings",
		total: XX.XX
		type: "equity"
	],
}
```

### endpoint get(/income-statement)

From:

Export JSON: *incomeStatement*

```js
{
	[
		type: "revenue",
		category: "Sales",
		value: 100000.00
	],
	[
		type: "cost",
		category: "Cost",
		value: 500.00
	],
	[
		type: "expense",
		category: "Expense",
		value: 1000.00
	]
}
```