---
tags: front-end
---
### Entries

Instructions: Xxxxxx xxxxxx xxxxx...

 | 
--- | ---
Type | [] Deposit [] Withdraw
Date |
Account |
Category |
Value |
Description |

 | 
--- | ---
Submit Entry | Clear

*Error field...*

Date | Account | Category | Value | Description
--- | --- | --- | --- | ---
 |
  |


### Balance
A | L
--- | ---
 0 | 0

 | 
--- | ---
Close & Submit |

*Error field...*


---

### Form Data

Get from: [[scripts/entries]]
```js
{
	[
		accountID: 1
		accountName: "Cash"
	],
	[
		accountID: 2
		accountName: "Bank Account"
	]
},
{
	[
		categoryID: 1
		categoryName: "Sales"
	],
	[
		categoryID: 2
		categoryName: "Cost"
	]
}
```

---

### Form Validation
Idea is to use HTML validation here
- Check if we have Date
- Check if we have Account
- Check if value is not 0
- Check if we have description

---
### Submit Entry Button

1. Check data validation
2. If OK, add data from form to table.
3. If entry contains category, add an automatic entry for "Earnings / Loss"
4. Sum added value to balance.
5. Add information to *Data Array*
6. If error, show error

---
### Clear Button
1. Clear form
2. Clear *Data Array*

---
### Close & Submit

1. Check balance (must be equal both sizes)
2. Apply similar form validation to *Data Array* before submit
3. If error, show error
4. If ok, show submit OK