---
title: Round Field Value
date: 2018-01-22T16:07:50+09:00
weight: 1450
---
## Summary

Rounds the specified field value to Round.

## How to use

### Parameters to set

Set FieldDigits.

#### field

Select the field to round. Only numeric fields can be selected.

#### Digits

Enter the number of digits to round. Entering a negative number results in a decimal point.

```
# Set "-2"
111.114 -> 111.11
111.115 -> 111.12

# Set "2"
140 -> 100
150 -> 200
```
