---
title: Calculate Fiscal Year
date: 2018-01-22T16:07:50+09:00
weight: 1460
---
## Summary

Calculates the year for a given date. Results can be viewed from other actions.

## How to use

If you want the result of the calculation to be in a separate field, select it in the Set To Field (optional) parameter.

Use a formula if you want to use it in other actions instead of immediately putting the result into a field.

When you perform an action set to “Calculate year”, the date is stored internally as a result of the action.

The saved year can be retrieved using a formula, for example, = $1.

Example) Change the resulting year to another action (see[Add records](../../record/insert_record/)“) for example

1.	Assume that the action number is number 1.
2.	“”[Add records](../../record/insert_record/), enter “= $1” for the field you want to set.(If the action number for “Calculate fiscal year” is number 2, “= $2” is assumed.)

### Parameters to set

Set the Date, Year Start Month, and Set To Field (optional).

#### Date

Enter the date for which you want to calculate the year.

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

#### Year Start Month

Select the year start month.

For example, if you select October for this month, October 2018 to September 2019 will be considered as 2018.

#### Set to field (optional)

Specify if you want to set the result of a calculation to another field. You can omit it it if you do not want to set the result directly to the field, but you want to use the result in another action.
