---
title: Calculate Date
date: 2018-01-22T16:07:50+09:00
weight: 1450
---
## Summary

Adds or subtracts days, months, and years to a date. The results can be viewed from other action.

## How to use

When you perform an action set to Calculate Dates, the date is stored internally as a result of the action.

You can use a formula to get the saved date, for example, = $1.

The saved date is in a format that can be set directly into the kintone date field. However, there is no time information, so you cannot set it to a date and time field.

Example) How to Set a Date in a Field

1.	Set up “Calculate date”. The action number is number one.
2.	[Set a value in a field](../../field/set_field_value), enter = $1 in Value. (If the action number for “Calculate date” is number 2, set “= $2”)

### Parameters to set

Specify the Base Date, Right Side Value, and Calculated Content.

#### Base Date

Enter the date on which you want to base.

If you want to refer to the value of a date or time field

```
=Date_2
```

Refer to the field code with “=” as shown in.

If you want to use the current date, use

```
=today()
```

in the Value field.

#### Right Value

The number of days, months, and years that you want to add.

For example, if you want to calculate “3 months after the base date”, select “X months after” in “Calculated content” and set “Right side value” to “3”.

You can also enter negative values. If “Right side value” is set to “-3” and “Calculation content” is set to “X months later”, then “3 months before the base date” will be calculated.

#### Calculated

Select from [X days after], [X weeks after], [X months after], or [X years after].
