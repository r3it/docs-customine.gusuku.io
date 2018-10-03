---
title: レコードを更新または追加する
date: 2018-01-22T16:07:50+09:00
weight: 1775
---
## Summary

Updates any records that match the key for the specified app, otherwise adds a new record.

## How to use

### Parameters to set

Set “Add to App”, “Key Field”, “Key Value”, and “Mapping”.

#### Add to App

Select the app for which you want to add or update records.

#### Key Fields

Select the field you want to use to retrieve records from.  
You cannot select a field in a table.

#### Key Value

Enter the key value of the record you want to retrieve.

#### Mapping

Enter the information you want to register for the record.

For more information on how to write this parameter, see [How to Write Field Mappings](../../field_mapping/) for more information.

## Limitations

Values cannot be registered for the following fields:

-	Checkbox
-	Multi-selection
-	Attachments
-	User Selection
-	Organization Selection
-	Group Selection
-	Table

### About Conflict Detection

If there is a record that matches the key, it attempts to save over that record, but checks for update conflicts.

This is similar to what you do.[Update records](../update_record/), you can choose whether to check for update conflicts in your settings. You cannot prevent this Update or Append Record from checking for conflicts.

On the other hand, if there is no record matching the key, that is, **Conflicts are not checked when a new record is created**.

Therefore, if two people perform the action at the same time, you might have two new records with the same content. If you don't want to do this, we strongly recommend that you leave “Prevent duplicate values” on the key fields in your kintone app settings.
