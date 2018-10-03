---
title: when a specified CALC field value changes
date: 2018-01-22T16:07:50+09:00
weight: 1072
---
## Summary

Performs an action when the value of a calculated field changes.

## How to use

Similar conditions include [When you edit the value of a field and the value changes](../when_field_change), but calculation fields cannot be edited directly. You cannot select a calculated field in “When the value changes by editing the value of the field”.

You can also change the field from which the calculation field is calculated to [When you edit the value of a field and the value changes](../when_field_change), you can also use this for the newly calculated value cannot be retrieved because the field has not been calculated yet.

“When the value of the calculated field changes” can be used to detect when the calculated value has actually changed, and the calculated value can also be retrieved.

### Parameters to set

Set the Fields.

#### field

Select a calculated field.Multiple selections are allowed, in which case the action is performed when the value of one of the selected fields changes.

## Limitations

Only the Add Record screen and Edit Record screen are supported.

It does not correspond to fields (columns) in the table.

It is not supported when editing by pressing the pencil button on the list screen.
