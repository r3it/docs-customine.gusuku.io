---
title: 指定の日付が指定の曜日ならば
date: 2018-03-26T14:53:50+09:00
weight: 1100
---
## Summary

The condition is met if the specified date is a specific day of the week.

## How to use

This condition is used in conjunction with other “when” conditions.

For example, if you open the screen and show a message if it's Monday today. [When the list screen is displayed](../../condition_event/when_record_list_show)“.

### Parameters to set

Set the Date and Day of the Week.

#### Date

Enter date data.

If you want to refer to the value of a date or time field

```
=Date_2
```

Refer to the field code with “=” as shown in.

To specify the current date, use the

```
=today()
```

in the Value field.

#### Day of the week

Select the day of the week.
