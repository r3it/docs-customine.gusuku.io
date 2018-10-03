---
title: フィールドの値を切り捨てる
date: 2018-01-22T16:07:50+09:00
weight: 1430
---
## Summary

Rounds the specified field value to Truncate.

## How to use

### Parameters to set

Set FieldDigits.

#### field

Select the field that you want to truncate. Only numeric fields can be selected.

#### Digits

Enter the number of digits to be truncated. Entering a negative number results in a decimal point.

```
# Set "-2"
111.119 -> 111.11

# Set "2"
190 -> 100
```
