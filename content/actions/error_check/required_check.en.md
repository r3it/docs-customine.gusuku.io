---
title: Check Required
date: 2018-01-22T16:07:50+09:00
weight: 1260
---
## Summary

Performs mandatory checks for the field. Sets the error message if the field is not entered or selected.

## How to use

### Parameters to set

Set FieldError Message.

#### field

Select which fields to check.

-	If you select more than one field, all of them are checked individually.
-	If you specify a field in a table, in special cases (*1), all rows in the table are checked.

\(*1) On the condition side, if there is a condition that restricts the table row, such as “When the value changes by editing the value of the field”, only those rows are checked.

#### Error message

Enter the error message to display if there are errors.

## Limitations

The following field type **CAN NOT** be used:

-	Table
-	Space
-	Groups
-	List of related records
-	Record Number
-	Author
-	Created at
-	Modified By
-	Modified
-	Category
-	Status
-	Worker

## Known Issues

If you select a field in the Attachment format, An issue has been identified that does not cause an error even if no attachments are attached.
