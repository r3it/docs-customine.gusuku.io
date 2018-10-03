---
title: Ser Error if Field Contains Two or More Value
date: 2018-01-22T16:07:50+09:00
weight: 1330
---
## Summary

Sets an error in the field when two or more items are selected in a multi-selection field, such as a checkbox.

Use this when you want to limit the selection to one.

## How to use

### Parameters to set

Set FieldError Message.

#### field

Select which fields to check.

-	If you select more than one field, all of them are checked individually.
-	If you specify a field in a table, in special cases (* 1), all rows in the table are checked.

\(* 1) On the condition side, if there is a condition that restricts the table row, such as “When the value changes by editing the value of the field”, only those rows are checked.

#### Error message

Enter the error message to display if there are errors.

## Limitations

You can only select one of the following types of fields:

-	Checkbox
-	Multi-selection
-	Attachments
-	User Selection
-	Group Selection
-	Organization Selection
-	Worker
-	Table

Attachment fields (which are columns) in a table are not supported on the record edit screen and add screen. In this case, regardless of the actual number of attachments, the system determines that it is not an error and does not set the error message.

Attachment fields are also correctly determined if they are outside the table.
