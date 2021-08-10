---
tags: script front-end
---
Execute getFormData() at script/page load.

### Variable list
var | type
--- | ---
*entry* | Object
*entryList* | Array

---
### function getFormData()

Get data from: [[back-end]]

Export JSON: *formData*

[[back-end#^640001]]

---
### function checkData()

1. Check if we have Date
2. Check if we have Account
3. Check if value is not 0
4. Check if we have description

**Return:** true | false

---
### function submitEntry(entry)


>1. Apply checkData(entry)
>2. If OK, add information to *entryList*
>3. Check if entry contains category: if so add an automatic entry for "Earnings / Loss" directly to *entryList*
>5. For each entryList, sum added value to balance.
>6. Aaaaa 
>7. If error, show error

^f3f987

Get data from: [[back-end]]
Export JSON: *formData*

---
### function clearForm()

1. Clear form
2. Clear *entryList*

Get data from: [[back-end]]

Export JSON: *formData*

---
### function postEntry()

1. Check balance (must be equal both sizes)
2. Apply similar form validation to *entryList* before submit
3. Post
4. If error, show error
5. If ok, show submit OK

Get data from: [[back-end]]

Export JSON: *formData*

---
