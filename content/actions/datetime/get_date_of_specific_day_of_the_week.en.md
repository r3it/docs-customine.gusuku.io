---
title: Get date of specific day of the week
date: 2018-01-22T16:07:50+09:00
weight: 1410
---
## Summary

Gets the date of a specific day of the week relative to today so that other actions can reference it.

## How to use

If you perform an action set to “Get the date of a specific day of the week”, the date will be stored internally as a result of the action.

You can use a formula to get the saved date, for example, = $1.

The saved date is in a format that can be set directly into the kintone date field.

Example) How to set a retrieved date to a field

1.	Set “Get dates for a specific day of the week”. The action number is number one.
2.	“”[Set a value in a field](../../field/set_field_value), enter = $1 in Value.(If the action number for “Get a specific day of the week” is number 2, say “= $2”)

### Parameters to set

Set the Target and Day of the Week.

#### Target

Choose from Week's, Next Week's, Last Week's, Next, or Previous.

The beginning of the week is calculated as Sunday.For example, if today is Wednesday 2018-07-04, this Sunday will be Sunday 2018-07-01.

“Next” does not mean next week, but it means the next day of the week. The same is true for “before”.For example, if today is Wednesday 2018-07-04, then “Next Friday” would result in 2018-07-06 (Fri).On the other hand, “Next Friday” will be 2018-07-13 (Fri).

Do not include “Next” today. The same is for “before”.For example, if today is Wednesday 2018-07-04 and you specify Next Wednesday, the result would be 2018-07-11 instead of Wednesday 2018-07-04.

#### Day of the week

Specifies the day of the week.

## Limitations

-	The standard today's date is based on the time zone (time difference) set for the “Time Zone” in the profile settings of the user logging into kintone.It cannot be fixed to a specific time zone (e.g. Japanese time).
