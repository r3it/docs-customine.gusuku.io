---
title: レコードを更新する
date: 2018-01-22T16:07:50+09:00
weight: 1770
---
## Summary

Update one record in the kintone app.

## How to use

### Parameters to set

Set “Destination app”, “Key field”, “Key value”, “Mapping” and “Check for update conflicts”.

#### Destination App

Select the app whose records you want to update.

#### Key Fields

Select a key field to update the record.  
You cannot select a field in a table.

#### Key Value

Enter a key value for the record you want to update.

#### Mapping

Enter the information you want to register for the record.

Each field you want to register is described in the form of “Registration destination field code = value to set”.

For more information on how to write this parameter, see [How to Write Field Mappings](../../field_mapping/) for more information.

#### Check for update conflicts

Select “Check” or “Do not check”.

Check checks for update records that conflict with updates from other users, and errors at run time. If it is not checked, this check is not performed.

If you are not sure, it is recommended to “check”.
