---
title: テーブルに行を追加または削除した時
date: 2018-01-22T16:07:50+09:00
weight: 1077
---
## Summary

Performs an action when a row is added or deleted from a table.

## How to use

A condition that performs an action when a user adds or deletes a row by pressing the “+-” button on the Add or Edit screen of a record.

When you use [Add a row to a table](../../../actions/table/add_table_row/), or [Delete a row from a table](../../../actions/table/remove_table_row/), this condition does on fire.

When you use [Export records to a table](../../../actions/table/write_record_to_table/), this condition does not fire.

It can be activated whether it is a PC screen or a smartphone screen.

### Parameters to set

Set up the Table.

#### Table

Select the table.
Multiple selections are allowed, in which case the action is performed when a row is added or deleted in one of the selected tables.

## Limitations

When you use [Spread a table](../../../actions/table/set_handsontable/), this condition does not fire.
