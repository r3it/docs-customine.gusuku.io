---
title: If Status is Specified
date: 2018-03-06T15:41:48+09:00
weight: 1020
---
## Summary

The action is executed when record status value has a specific CONDITION.

## How to use

### Parameters to set

Set “CONDITION” and “Comparison value”.

#### Condition

The following could be selected for “CONDITION”:

| Condition Name  | Condition definition                                                          |
|:----------------|:------------------------------------------------------------------|
| Even | In case when the specified field value matches the comparison value |
| Uneven | In case when the specified field value does not match the comparison value |

#### Comparison Value

Set a value to compare with field value.
One of the following values could be specified.

- Direct input
Directly input the comparison value.
- Field selection
Compare to the other field value within the same record.
- Other action result
Compare to the result value of already-registered action.

### About comparison process
 - Spaces before and after the value are ignored at comparison.
 - Text is compared by using Unicode value based on standard lexicographic order.
 However, double byte, single byte, and upper/lower case are not classified.

## Limitations

Not available on the Add Record screen.
