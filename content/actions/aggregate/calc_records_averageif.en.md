---
title: Average of Field that meets Criteria.
date: 2018-01-22T16:07:50+09:00
weight: 1150
---
## Summary

The action calculates the average value of the field specified from the pre-obtained record which fulfills a specific CONDITION.
The calculated result could be used in different actions.

## How to use

### Parameters to set

Set “Record selecting action”, “Field to calculate”, “CONDITION decision field”, ”CONDITION” and “Comparison value”.

#### Record Selection Actions

From the action list, select the action which obtained the record for calculation.

#### Calculated fields

Select the field for calculating average value, “Number” or “Calculated field”s.

#### Condition fields

From the Apps field, select the field for deciding the CONDITION.
Fields within the table can not be selected.

#### Condition

Select “CONDITION” from the following selection.

<a href="https://support.gusuku.io/ja-JP/support/solutions/articles/36000045806" target="_blank"> Refer here for field CONDITION list</a>.

#### Comparison Value

Set a value to compare with field value.
One of the following values could be specified.

- Direct input
Directly input the comparison value.
- Field selection
Compare to the other field value within the same record.
- Other action result
Compare to the result value of already-registered action.

### About comparison process

- Spaces before and after the value are ignored at comparison.
- Text is compared by using Unicode value based on standard lexicographic order.
 However, double byte, single byte, and upper/lower case are not classified.

#### Field to set result (optional)

Specify this when setting the calculation result to another field. If you do not set it in the direct field but want to use the calculation result in another action, you can omit it.

## Things to Note

Calculated results are not rounded.
Refer to “[Rounding field value](../../field/round4d5u_field)” for displaying the rounded result.
