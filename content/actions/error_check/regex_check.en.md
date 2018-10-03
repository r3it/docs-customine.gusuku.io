---
title: Check with Regular Expression
date: 2018-01-22T16:07:50+09:00
weight: 1290
---
## Summary

Checks whether a field conforms to a specific format using string pattern matching called a regular expression.

You will need some knowledge of “regular expressions”.

## How to use

### Parameters to set

Set Field Regular Expression Error Message.

#### field

Select which fields to check.

-	If you select more than one field, all of them are checked individually.
-	If you specify a field in a table, in special cases (* 1), all rows in the table are checked.

\(* 1) On the condition side, if there is a condition that restricts the table row, such as “When the value changes by editing the value of the field”, only those rows are checked.

#### Regular expression

Enter the regular expression to check.If this regular expression is not matched, it is considered an error.

#### Error message

Enter the error message to display if there are errors.

## Limitations

You can only select one of the following types of fields:

-	String (one line)
-	String (multiple lines)
-	Rich Editor
-	Link
