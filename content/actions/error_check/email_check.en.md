---
title: Check E-mail address format.
date: 2018-01-22T16:07:50+09:00
weight: 1280
---
## Summary

Checks whether the specified field is in email address format.

Displays an error message in the field as a result of the check.

## How to use

### Parameters to set

Set “Field”, “Check Accuracy” and “Error Message”.

#### field

Select whether to check the field.

-	If you select more than one field, all of them are checked individually.
-	If you specify a field in a table, in special cases (* 1), all rows in the table are checked.

\(* 1) On the condition side, if there is a condition that restricts the table row, such as “When the value changes by editing the value of the field”, only those rows are checked.

#### Check Accuracy

Choose how granular you want to check.

-	Exclusive... It also checks for characters that can be used. (*)
-	Loosen... just check for the presence of” @”.

\(*) This is not a complete, even if it is true. Even if the address is violating the RFC, the check may pass.

#### Error message

Enter the error message to display if there are errors.

### Limitations

You can only select one of the following types of fields:

-	String (one line)
-	String (multiple lines)
-	Rich Editor

You cannot specify a field in a table and a field outside the table at the same time, or a field in a different table at the same time. If you want to check fields in and out of a table or in different tables at once, you can separate them into multiple actions.
