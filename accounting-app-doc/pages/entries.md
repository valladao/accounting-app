---
tags: front-end
---
## Page Visual
### Entries

Instructions: Xxxxxx xxxxxx xxxxx...

 | 
--- | ---
Type | [] Deposit [] Withdraw
Date |
Account | Select _formData_
Category | Select _formData_
Value |
Description |

 | 
--- | ---
Submit Entry | Clear

*Error field...*

Date | Account | Category | Value | Description
--- | --- | --- | --- | ---
 entryList[x].date | entryList[x].account | entryList[x].category | entryList[x].value | entryList.description
...  | ... | ... | ... | ...


### Balance
A | L
--- | ---
 0 | 0

 | 
--- | ---
Close & Submit |

*Error field...*


---
## Page Control

### Form Data
Function: getFormData()
Get from: [[scripts/entries]]

[[back-end#^640001]]

---

### Form Validation
To use HTML validation here
- Check if we have Date
- Check if we have Account
- Check if value is not 0
- Check if we have description

---
### Submit Entry Button
Variables: entry (Object attached in form inputs)
Function: submitEntry(entry)
Done by: [[scripts/entries]]

[[scripts/entries#^f3f987]]

---
### Clear Button
Function: clearForm()
Done by: [[scripts/entries]]

1. Clear form
2. Clear *Data Array*

---
### Close & Submit
Function: postEntry()
Done by: [[scripts/entries]]

1. Check balance (must be equal both sizes)
2. Apply similar form validation to *Data Array* before submit
3. Post
4. If error, show error
5. If ok, show submit OK