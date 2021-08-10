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

From: [[migrations/income-statement]]

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

### endpoint get(/form-data)

Get data from: [[accounts]] and [[categories]]

Export JSON: *formData*

```js
{
	[
		accountID: 1,
		accountName: "Cash",
		accountType: "assets"
	],
	[
		accountID: 2
		accountName: "Bank Account"
		accountType: "assets"
	]
},
{
	[
		categoryID: 1
		categoryName: "Sales"
		accountType: "equity"
	],
	[
		categoryID: 2
		categoryName: "Cost"
		accountType: "equity"
	]
}
```

^640001
