---
title: Ser Error if Field Value is not Half-Width
date: 2018-01-22T16:07:50+09:00
weight: 1330
---
## Summary

Examine the characters entered in the field and cause an error if they contain double-byte characters.

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

-	String (one line)
-	String (multiple lines)
-	Number
-	Rich Editor
-	Link
