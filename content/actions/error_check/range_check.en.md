---
title: Check Range of Number
date: 2018-01-22T16:07:50+09:00
weight: 1300
---
## Summary

Checks a numeric range in a numeric field.

This is similar to the check in the “number” itself of kintone.

Unlike the kintone standard checks, combined with conditions allows for more complex checks.

## How to use

### Parameters to set

Set Field, Minimum, Maximum, and Error Message.

#### field

Select which fields to check.

-	If you select more than one field, all of them are checked individually.
-	If you specify a field in a table, in special cases (* 1), all rows in the table are checked.

\(* 1) On the condition side, if there is a condition that restricts the table row, such as “When the value changes by editing the value of the field”, only those rows are checked.

#### Min Value

Enter the minimum value for that field.

#### Maximum value

Enter the maximum value for that field.

#### Error message

Enter the error message to display if there are errors.

## Limitations

You can only select one of the following types of fields:

-	Number
-	Calculation
