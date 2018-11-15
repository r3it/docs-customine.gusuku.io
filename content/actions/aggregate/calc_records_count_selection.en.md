---
title: Count Selection of Field of Records
date: 2018-01-22T16:07:50+09:00
weight: 1145
---
## Summary

Counts the number selected in the specified field of a record. The count results can be used in another action.

## How to use

Counts the number of selections in a field that allows multiple selections, such as a checkbox or user selection. If there is no selection, it is 0.

### Parameters to set

Set Record Selection Action, Field to Count, Equal Count Method, and Field to Set Result (Optional).

#### Record Selection Actions

From the list of actions, select the action that retrieves the records you want to calculate.

#### Fields to count

Select the fields you want to count.

You can only select fields that allow multiple selections, such as checkboxes or user selections, not attachment fields.

#### How to count the same values

If you select “Count Same Values Separately”, the number of selections is simply counted regardless of the selected value.

If you select Count Same As One, two or more rows that have the same value will be counted as one, i.e., “how many different values are chosen”.

For example, if you have three records, the value of the field to count is

-	Line 1: A, B, C
-	Line 2: X
-	Line 3: Y, Z, A

, then the

-	Count the same value separately, then the count value is 7 (3+3+1)
-	If you count the same value as 1, then the count value is 6 (A, B, C, X, Y, Z).

will be used as a result.

#### Field to set the result (optional)

Specify if you want to set the result of a calculation to another field. You can omit it it if you do not want to set the result directly to the field, but you want to use the result in another action.
