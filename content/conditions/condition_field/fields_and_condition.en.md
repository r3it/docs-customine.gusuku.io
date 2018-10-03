---
title: 複数フィールドが全て同じ条件を満たすならば
date: 2018-01-22T16:07:50+09:00
weight: 1100
---
## Summary

Action is executed depending on the result of the comparison between the specified field value and the comparison value.
The action is executed when multiple fields all fulfill the CONDITION.

## How to use

### Parameters to set

Set “Field”, “CONDITION”, and “Comparison value”.

#### Field

For “Field”, select the field name for comparing the value.

Multiple fields are selectable.

In case when multiple fields are selected, the action is executed when all the selected fields fulfil the CONDITION.
The action is not executed if 1 or more selected field do not fulfill the CONDITION.


#### Condition

The following could be selected for “CONDITION”:

<a href="https://support.gusuku.io/ja-JP/support/solutions/articles/36000045806" target="_blank">See a list of field criteria</a> for more information.

#### Comparison Value

Set field value and value for comparison.
One of the following values could be specified.

-	Direct input  
	Enter comparison value directly
-	Field Selection  
	Compares against other field values in the same record
-	Results of other actions  
	Compare to the result value of the registered action

### About the Comparison Process

- Spaces before and after the value are ignored at comparison.
- Text is compared by using Unicode value based on standard lexicographic order. 
 However, double byte, single byte, and upper/lower case are not classified.
