---
title: Minimum of Field that meets Criteria.
date: 2018-01-22T16:07:50+09:00
weight: 1180
---
## Summary

Calculates the smallest value in a field based on records that meet a specified criteria. Calculated results can be used in other actions.

## How to use

### Parameters to set

Set [Record Selection Action], [Calculation Field], [Condition Condition Field], [Compare Value], and [Value].

#### Record Selection Actions

From the list of actions, select the action that retrieves the records you want to calculate.

#### Calculated fields

Select the field for which you want to calculate the minimum value. You can select a number or a calculated field.

#### Condition fields

From the app fields, select the field you want to use to determine the condition. You cannot specify a field in a table.

#### Condition

Select a Condition from the following choices:

<a href="https://support.gusuku.io/ja-JP/support/solutions/articles/36000045806" target="_blank">See a list of field criteria</a> for more information.

#### Comparison Value

Compare Value to set the value against which the field value is compared. The comparison value can be one of the following values:

-	Direct input  
	Enter comparison value directly
-	Field Selection  
	Compares against other field values in the same record
-	Results of other actions  
	Compare to the result value of the registered action

##### About the Comparison Process

-	When comparing, leading and trailing spaces are ignored.
-	Strings are compared using Unicode values in standard lexical order. However, full-width, half-width and case are not sensitive.

#### Field to set result (optional)

Specify this when setting the calculation result to another field. If you do not set it in the direct field but want to use the calculation result in another action, you can omit it.
