---
title: Count Rows of Records that meets Criteria.
date: 2018-01-22T16:07:50+09:00
weight: 1190
---
## Summary

Calculates the number of rows in a previously retrieved record that satisfies the specified criteria. Calculated results can be used in other actions.

## How to use

### Parameters to set

Set [Record Selection Action], [Condition Condition], [Compare Value], and [Value].

#### Record Selection Actions

From the list of actions, select the action that retrieves the records you want to calculate.

#### Condition fields

From the app fields, select the field you want to use to determine the condition. You cannot specify a field in a table.

#### Condition

For Conditions, you can choose from the following choices:

<a href="https://support.gusuku.io/ja-JP/support/solutions/articles/36000045806" target="_blank">See a list of field criteria</a> for more information.

#### Comparison Value

Compare Value to set the value against which the field value is compared. The comparison value can be one of the following values:

-	Direct input  
	Enter comparison value directly
-	Field Selection  
	Compares against other field values in the same record
-	Results of other actions  
	Compare to the result value of the registered action

### About the Comparison Process

-	When comparing, leading and trailing spaces are ignored.
-	Strings are compared using Unicode values in standard lexical order. However, full-width, half-width and case are not sensitive.
