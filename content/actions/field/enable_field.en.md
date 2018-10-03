---
title: フィールドを有効化する
date: 2018-01-22T16:07:50+09:00
weight: 1360
---
## Summary

Restores fields that are in the disabled state (disabled state) to the original state for input.

## How to use

Fields that can not be entered in [Disable a field](../disable_field/) and a field which is a copy destination of the lookup field and which is not permitted to input,
You can return to the state that can be input.

If you execute “Enable Field” on a field that is originally available for input, nothing happens. It does not result in an error.

### Parameters to set

Set the Fields.

#### field

Select the field you want to enable.Multiple selections are allowed, and all selected fields are enabled at the same time.

## Limitations

The following field type **CAN NOT** be used:

-	Space
-	Table
-	Groups
-	List of related records
-	Author
-	Created at
-	Modified By
-	Modified
-	Category
-	Status
-	Worker
