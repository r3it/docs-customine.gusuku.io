---
title: Get Specific Date
date: 2018-01-22T16:07:50+09:00
weight: 1400
---
## Summary

Gets a specific date so that it can be referenced by other actions.

## How to use

When you perform an action set to Get a specific date, the date is stored internally as a result of the action.

You can use a formula to get the saved date, for example, = $1.

The saved date is in a format that can be set directly into the kintone date field.

Example) How to set a retrieved date to a field

1.	Set up “Get a specific date”. The action number is number one.
2.	[Set a value in a field](../../field/set_field_value), enter = $1 in Value. (If the action number for “Get a specific date” is number 2, say “= $2”)

### Parameters to set

Set the Date Type.

#### Date Type

Select the date you want to retrieve, such as Today or At the beginning of this month.

## Other methods

You can also use a function in a formula without using an action.

[Set a value in a field](../../field/set_field_value/) in the “Value” parameter, for example,

```
=getDate("今月月初")
```

You can specify a function, such as.

The “beginning of this month” part of the above example can be one of the following:

-	Today
-	Yesterday
-	Tomorrow
-	First of this month
-	End of this month
-	First of last month
-	Last month
-	First month
-	Last day of next month
-	First of this year
-	End of this year
-	First of last year
-	End of last year
-	Early next year
-	End of next year
-	Year 1
-	End of fiscal year
-	First Day of Last Year
-	Last Year
-	First Day of Next Year
-	Next Year End

## Limitations

-	The standard today's date is based on the time zone (time difference) set for the “Time Zone” in the profile settings of the user logging into kintone. It cannot be fixed to a specific time zone (e.g. Japanese time).

-	In this “thing to do”, the range of “fiscal year” is fixed from April to March. It is not possible to get the start date of the year in a different year range.
