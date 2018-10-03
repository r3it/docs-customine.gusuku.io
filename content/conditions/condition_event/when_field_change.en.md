---
title: when a specified field value changes
date: 2018-01-22T16:07:50+09:00
weight: 1070
---
## Summary

Executes the action when the field value was changed from editing.

## How to use

A condition for executing the action when the field value was edited and changed by a user.

The action is invoked at the time the field is edited, even when the user has not yet saved the record.

The action is invoked in the View tab for both PC and smartphone.

In the PC Record View: the action is also invoked by pressing the “Pencil” button to edit the in-line field of the record within the “View” tab.

### Parameters to set

Set “Field” and “When pressing the Pencil in View tab”.

#### Field

Select which field to edit for executing the action.
Multiple fields are selectable. In that case, the action is executed when the value in 1 of the fields was changed.

#### When pressing the Pencil in View tab

Select whether or not to invoke the condition when editing the field by pressing the Pencil button in the View tab.

By selecting “Include also when pressing the Pencil button in the View tab”, this CONDITION is also invoked when the Pencil button is pressed to edit.

By selecting “Do not include when pressing the Pencil button in the View tab”, this CONDITION will not be invoked when the Pencil button is pressed to edit.

## Limitations

Currently, the action is invoked only by selecting the following field type: 

For more details, please refer to:
[https://developer.cybozu.io/hc/ja/articles/201941984#step3](https://developer.cybozu.io/hc/ja/articles/201941984#step3)

-	Radio buttons
-	Drop-down
-	Checkbox
-	Multi-selection
-	User Selection
-	Organization Selection
-	Group Selection
-	Date
-	Time
-	Date and time
-	String (one line)
-	Number

In addition to the above, Customine also supports the following fields:

-	String (multiple lines)
-	Link

“String (multiple lines)” “Link” does not fire when the value is copied in the lookup.

### About Calculated Fields

You cannot specify a calculated field in this “When the value changes by editing the value of the field”.

Also, if you specify the field from which the calculated field is calculated, Calculated Fields Are Recalculated **Previous** condition is triggered.

For example, if a calculation field is set to

```
Number_1 + Number_2
```

if it was.

Then, in the field “When the value changes by editing the value of the field,” “Number_1” “Number_2” is specified.

First, “Number_1 = 10” “NumberThe value of _2 = 20” is 30 in the calculated field.where the user is “NumberYou changed the value of _1” to 100.

When you do so, the condition “When the value changes by editing the value of the field” is triggered. At this moment, the value of the calculated field is **We haven't changed yet.** If you try to do something using the value in the calculated field at this time, you get the previous value 30. Expected to have 100+20 120 and behave wrong.

If you want to do something when the value of a calculated field changes, see[When the value of a calculated field changes](../when_calc_changed/) for more information. As the name suggests, you can get the calculated value.
