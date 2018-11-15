---
title: Get date of specific day of the week
date: 2018-01-22T16:07:50+09:00
weight: 1410
---
## Summary

Gets the date of a specific day of the week relative to today so that other actions can reference it.

## How to use

If you want to include the retrieved date in the field, select that field in the "Destination field (optional)" parameter.

If you want to use the acquired date in another field instead of putting it in the field immediately, use the formula.

If you perform an action set to “Get the date of a specific day of the week”, the date will be stored internally as a result of the action.

You can use a formula to get the saved date, for example, = $1.

The saved date is in a format that can be set directly into the kintone date field.

Example) An example of using the acquired date as another action ("[Add record](../../record/insert_record/)")

1.	Set “Get dates for a specific day of the week”. The action number is number one.
2.	In "Mapping" of [Add record](../../record/insert_record/), put "=$1" in the date field you want to set. (If the action number for “Get a specific day of the week” is number 2, say “= $2”)

### Parameters to set

Set the Target and Day of the Week.

#### Target

Choose from Week's, Next Week's, Last Week's, Next, or Previous.

The beginning of the week is calculated as Sunday.For example, if today is Wednesday 2018-07-04, this Sunday will be Sunday 2018-07-01.

“Next” does not mean next week, but it means the next day of the week. The same is true for “before”.For example, if today is Wednesday 2018-07-04, then “Next Friday” would result in 2018-07-06 (Fri).On the other hand, “Next Friday” will be 2018-07-13 (Fri).

Do not include “Next” today. The same is for “before”.For example, if today is Wednesday 2018-07-04 and you specify Next Wednesday, the result would be 2018-07-11 instead of Wednesday 2018-07-04.

#### Day of the week

Specifies the day of the week.

#### Set destination field (optional)

Specify this when setting the acquired date in another field. If you do not set it in the direct field and you want to use the result in another action, you can omit it.

## Limitations

-	The standard today's date is based on the time zone (time difference) set for the “Time Zone” in the profile settings of the user logging into kintone.It cannot be fixed to a specific time zone (e.g. Japanese time).
