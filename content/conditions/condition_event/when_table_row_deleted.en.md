---
title: テーブルから行を削除した時
date: 2018-01-22T16:07:50+09:00
weight: 1076
---
## Summary

Executes an action when a row is deleted from the table.

## How to use

A condition that performs an action when a user deletes a row by pressing the button on the Add or Edit screen of a record.

When you use [Delete a row from a table](../../../actions/table/remove_table_row/), this condition does on fire.

When you use [Export records to a table](../../../actions/table/write_record_to_table/), this condition does not fire.

It can be activated whether it is a PC screen or a smartphone screen.

It does not fire when adding rows.

### Parameters to set

Set up the Table.

#### Table

Select the table. Multiple selections are allowed, in which case the action is performed when a row is deleted in one of the selected tables.

## Limitations

When you use [Spread a table](../../../actions/table/set_handsontable/), this condition does not fire.
