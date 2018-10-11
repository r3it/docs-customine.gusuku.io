---
title: Calculate Age
date: 2018-01-22T16:07:50+09:00
weight: 1530
---
## Summary

Calculates age based on a date field and sets it to another field.

## How to use

The age is calculated by the date at which the action was performed and the age at the end of the birth date.

The date on which the action was performed is based on the regional settings of the user's browser. If you are using a Japanese browser, it will be in Japan time.

### Parameters to set

Set the Date or Date Time Field and Age Set Field.

#### Date or datetime field

Select a date or time field that contains a date that represents a birthday.

If you select a datetime field, the time is not considered in the calculation.

#### The field to set the age

Specifies the field in which to set the result of the calculation.

The available field types are:

-	String (one line)
-	String (multiple lines)
-	Rich Editor
-	Number

## Limitations

The Current Date is based on the time zone setting of the logged-in user. The time zone is set to “(UTC+09: 00) In the case of Osaka, Sapporo and Tokyo”, it will be Japan time.
