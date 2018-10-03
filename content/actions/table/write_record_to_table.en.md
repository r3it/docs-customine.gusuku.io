---
title: レコードをテーブルに書き出す
date: 2018-03-06T12:01:14+09:00
weight: 1010
---
## Summary

Export record data to a table in this app.

## How to use

Used with [Retrieve records by specifying criteria](../../record/get_records_by_query), etc., you can export records to a row in a table.

The original record can be from another app, or you can use the [Fetch a table row as a record](../get_record_from_table).

By connecting “Fetch table rows as records” and “Export records to table”, you can copy table data in your app.

### Parameters to set

Set Destination Table, Records, Mapping, Existing Rows.

#### Destination Table

Select the table you want to export to.

#### Record

Select the action that retrieved the record data from which you want to export.

#### Mapping

Sets the field (column) values for the table to be exported.

For more information on how to write this parameter, see [How to Write Field Mappings](../../field_mapping/) for more information.

If you leave a field empty, you do not export the empty value, but do not export the field. For updates, the values from the original record are preserved, and for inserts, the initial values from the app settings are set.

#### Existing Rows

Choose whether to clear the original rows in the destination table or append them without clearing them.

## Limitations

You cannot export to fields outside the table.
