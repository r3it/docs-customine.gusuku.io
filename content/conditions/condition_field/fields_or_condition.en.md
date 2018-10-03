---
title: 複数フィールドのうちどれか１つか条件を満たすならば
date: 2018-01-22T16:07:50+09:00
weight: 1110
---
## Summary

Determines whether or not the action is performed by comparing the value of the specified field to the compare-to value. Perform an action if at least one of the fields satisfies the condition.

## How to use

### Parameters to set

Set Field Conditional Compare Value.

#### field

For Field, select the name of the field whose values you want to compare.

You can select multiple fields.

If multiple selections are made, the action is performed if at least one of the selected fields satisfies the condition. If all of the selected fields do not meet the criteria, no action is taken.

#### Condition

For Conditions, you can choose from the following choices:

<a href="https://support.gusuku.io/ja-JP/support/solutions/articles/36000045806" target="_blank">See a list of field criteria</a> for more information.

#### Comparison Value

Compare Value to set the value against which the field value is compared.  
The comparison value can be one of the following values:

-	Direct input  
	Enter comparison value directly
-	Field Selection  
	Compares against other field values in the same record
-	Results of other actions  
	Compare to the result value of the registered action

### About the Comparison Process

-	When comparing, leading and trailing spaces are ignored.
-	Strings are compared using Unicode values in standard lexical order.  
	However, full-width, half-width and case are not sensitive.
