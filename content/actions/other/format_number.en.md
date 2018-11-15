---
title: Format Number
date: 2018-01-22T16:07:50+09:00
weight: 1510
---
## Summary

Converts numeric data to the specified format.

## How to use

The source data of a number can refer to the results of a field or other action using an expression.

If you want to put formatted results in another field, select that field in the "Set destination field (optional)" parameter.

Instead of placing formatted results in the field immediately, if you want to use it in other actions, use mathematical expressions.

The resulting string is set as the result of the action.

If you want to retrieve the result, use an expression to reference this action in other actions.

For example, if the action “format numbers” is number 1, [Set a value in a field](../../field/set_field_value/) in the “Value” parameter, for example,

```
=$1
```

to retrieve it.

You can also use expressions to add strings such as unit symbols before and after the result.

```
="Market price " & $1 & " Yen"
```

as follows:

### Parameters to set

Numer_Show Thousands Separators, Number of Decimal Digits, Zero-padded, Decimal Digits, and Zero-padded Decimals.

#### Number

Specifies a numeric value.

If you want to see values in other fields

```
=Number_2
```

Refer to the field code with “=” as shown in.

At this time, it is also possible to perform the arithmetic operation with the equation.

```
=Number_2 * 100
```

#### Show Thousands Separator

Show Thousands Separator to display commas every three digits of the integer part.

#### Number of digits in the integer part

Specifies the number of digits to display for the integer portion. This number does not include commas for thousands separators or decimal places.

If the number exceeds this number of digits, the number of high-order digits is not displayed. For example, if you specify “Number of Digits” as “3”, only the last three digits will be displayed.

If none is specified, the integer portion is displayed without cutting digits or padding zeros.

#### Zero-padding of whole numbers

If you specify Number of Decimal Places, specify whether to zero if the number is less than the number of digits.

If you do not specify the number of digits in the integer part, this parameter is ignored.

If “Number of digits” is “5” and the number is “512”, padding zeros results in “00512”.

You can combine integer zero padding and comma separators. If both comma-delimited and zero-padded are set to “Yes”, the bottom portion of the zero-padded will also contain commas. For example, if “Number of digits” is “5” and the number is “1512”, then “01,512” is.

#### Decimal Places

If this number of digits is specified, the number of digits is truncated to the nearest decimal point.

If not specified, all internal digits are displayed.

#### Zero-padding for fractional parts

If Decimal Places is specified, specifies whether to pad zero if less than the specified number of digits.

If Decimal Places is not specified, this parameter is ignored.

For example, if Decimal Places is 3 digits and the number is 0.5, the result is 0.500.

#### Field to set result (optional)

Specify this when setting the calculation result to another field. If you do not set it in the direct field but want to use the calculation result in another action, you can omit it.
