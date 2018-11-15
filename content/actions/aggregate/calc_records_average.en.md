---
title: Average of Field of Records
date: 2018-01-22T16:07:50+09:00
weight: 1100
---
## Summary

Calculates the average of previously retrieved records in a specified field. Calculated results can be used in other actions.

## How to use

### Parameters to set

Set Record Selection Action Field to Calculate.

#### Record Selection Actions

From the list of actions, select the action that retrieves the records you want to calculate.

#### Calculated fields

For Field to Calculate, select a numeric field or any field from the calculation field.However, you cannot select a field in the table.

#### Field to set result (optional)

Specify this when setting the calculation result to another field. If you do not set it in the direct field but want to use the calculation result in another action, you can omit it.

## Precautions

It does not round the results of the calculation. Separate [Round the value of a field](../../field/round4d5u_field), and so on.
