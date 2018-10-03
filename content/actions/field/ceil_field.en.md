---
title: フィールドの値を切り上げる
date: 2018-01-22T16:07:50+09:00
weight: 1440
---
## Summary

Rounds the specified field value with Round Up.

## How to use

### Parameters to set

Set FieldDigits.

#### field

Select the field that you want to round up. Only numeric fields can be selected.

#### Digits

Enter the number of digits to round up. Entering a negative number results in a decimal point.

```
# Set "-2"
111.111 -> 111.12

# Set "2"
110 -> 200
```
