---
title: レコードを書き出す
date: 2018-01-22T16:07:50+09:00
weight: 1778
---
## Summary

You can export the records with [Retrieve records by specifying criteria](../get_records_by_query/) or other action that retrieves records.

You can export field values in the same app as you rewrite them, or you can export them as new records in a separate app.

## How to use

### Parameters to set

You must set action like a [Retrieve records by specifying criteria](../get_records_by_query/) for retrieve records.

Set Record, Export To App, Mapping, Update or Insert.

#### Record

Specifies the action that retrieved the record from which you want to export.

#### Export to

Select the app you want to export to.

It can be the same app as the original record, or it can be a different app.

#### Mapping

Sets the field values for the records you want to export.

For more information on how to write this parameter, see [How to Write Field Mappings](../../field_mapping/) for more information.

If you leave a field empty, you do not export the empty value, but do not export the field.For updates, the values from the original record are preserved, and for inserts, the initial values from the app settings are set.

In this “Export Records” mapping, the fields listed under “Set Values” become the fields in the app of the record you are exporting from.

#### Update or Insert

Select “Update Existing Records” to overwrite the values in the same record as the export source.

Insert New Record creates and inserts another new record instead of overwriting.

For “Update Existing Records”, the source app and the destination app must be the same app.

### About Conflict Detection

Update Existing Records checks for update conflicts.

Insert Record New is not checked.
