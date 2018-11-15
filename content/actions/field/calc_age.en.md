---
title: Calculate Age
date: 2018-01-22T16:07:50+09:00
weight: 1530
---
## Summary

Calculates age based on a date field and sets it to another field.

## How to use

To set the calculated age in the field, create the field in the application and select that field in "Field to set age".

If you want to convert the calculated age to a field etc. by processing the format like 'full 30' instead of just a number, do as follows.

1. Do not set "age setting field" and skip it.
1. Set [Set value in field](../set_field_value) " and set its "value" as below using the calculation function.

```
= "Full" & $ 1 & "old"
```

- For part of $ 1, please specify the number of the action that set "calculate age". For example, if the action number is 3, it is $ 3.

The age is calculated by the date at which the action was performed and the age at the end of the birth date.

The date on which the action was performed is based on the regional settings of the user's browser. If you are using a Japanese browser, it will be in Japan time.

### Parameters to set

Set the Date or Date Time Field and Age Set Field.

#### Date or datetime field

Select a date or time field that contains a date that represents a birthday.

If you select a datetime field, the time is not considered in the calculation.

#### The field to set the age

Specify the field to set the calculation result. It is optional.

The available field types are:

-	String (one line)
-	String (multiple lines)
-	Rich Editor
-	Number

If omitted, the age is not set in the field. It is possible to reference from other actions even if omitted.

## Limitations

The Current Date is based on the time zone setting of the logged-in user. The time zone is set to “(UTC+09: 00) In the case of Osaka, Sapporo and Tokyo”, it will be Japan time.
