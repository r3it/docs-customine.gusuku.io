---
title: Calculate Period Number
date: 2018-01-22T16:07:50+09:00
weight: 1470
---
## Summary

Calculates the number of periods for a given date. The results can be viewed from other actions.

## How to use

If you want the result of the calculation to be in a separate field, select it in the Set To Field (optional) parameter.

Use a formula if you want to use it in other actions instead of immediately putting the result into a field.

When you perform an action set to “Calculate period”, the date is stored internally as a result of the action.

You can use a formula to get saved periods, for example, = $1.

Example) Change the result period to another action (see[Add records](../../record/insert_record/)“) for example

1.	Assume that the action number is number 1.
2.	“”[Add records](../../record/insert_record/), enter “= $1” for the field you want to set.(If the action number for “Calculate period” is number 2, “= $2” is assumed.)

### Parameters to set

Set Date, Year Start Month, Year First Period, and Set To Field (Optional).

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

#### Year of the first year

Enter the year for the first period as a numeric year.

For example, if the year starts in October and the year in the first period is 2000,

-	The date is October 2000 ⇒ 1
-	Date Sep 2001 ⇒ 1
-	The date is October 2001 ⇒ 2

is the result of the following:

#### Set to field (optional)

Specify if you want to set the result of a calculation to another field. You can omit it it if you do not want to set the result directly to the field, but you want to use the result in another action.

## Limitations

If the result is a date that is earlier than the start of the first period, the result may be zero or a negative value. Again, there is no error.
