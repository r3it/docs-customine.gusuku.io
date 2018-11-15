---
title: Format Date/Time
date: 2018-01-22T16:07:50+09:00
weight: 1500
---
## Summary

Converts date and time data to the specified format.

## How to use

You can use expressions to refer to the results of fields and other actions.

If you want to put formatted results in another field, select that field in the "Set destination field (optional)" parameter.

Instead of placing formatted results in the field immediately, if you want to use it in other actions, use mathematical expressions.

The resulting string is set as the result of the action.

If you want to retrieve the result, use an expression to reference this action in other actions.

For example, if the action “Format a date or time” was first, the [Set a value in a field](../../field/set_field_value/) in the “Value” parameter, for example,

```
=$1
```

to retrieve it.

### Parameters to set

Set Date/Time Date FormatsTime Format.

#### Date/Time

Specify a date or time value.

If you want to refer to the value of a date or time field

```
=Date_2
```

Refer to the field code with “=” as shown in.

If you want to see the current date and time

```
=now()
```

in the Value field.

#### Date Format

You can choose from several patterns.

Select “No Date Display” if the source data is only time and does not contain dates.

You can also select “No Date” if the source data contains a date, such as “Date and Time”.

#### Time Format

You can choose between 12-hour or 24-hour clock.

Select “No Time Display” if the source data is only a date and does not contain a time.

You can also select “No time display” if the source data contains time, such as “Date and Time”.

#### Field to set result (optional)

Specify this when setting the calculation result to another field. If you do not set it in the direct field but want to use the calculation result in another action, you can omit it.

## Other methods

You can also use functions to format formulas without using actions.

[Set a value in a field](../../field/set_field_value/) in the “Value” parameter, for example,

```
=format(Date_2, "YYYY/MM/DD")
```

You can specify the format function, as shown in.

The advantage is that you can format directly without any action, but you need to understand the rules of formatting specification like “YYYY/MM/DD” and it is a feature for advanced users.

As an application of this method, you can use the following formula to get the day of the week in a date field: The day of the week is displayed based on the locale settings of the user who is in kinone.

```
=format(Date_2, "dddd")
```
