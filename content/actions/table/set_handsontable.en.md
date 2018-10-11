---
title: Set Table Like Spreadsheet
date: 2018-01-22T16:07:50+09:00
weight: 1690
---
## Summary

Makes the table look similar to a spread (a spreadsheet application like Microsoft Excel or Google Spread).

![Handsontable](/images/ja/actions/table/set_handsontable/1.png)

## How to use

Please place a space field in your app before proceeding. The spread appears at this space location.

The displayed spread cannot be edited on the record details screen, but the contents can be edited on the record add screen or record edit screen.

If you add a row to the spread, the cell is in edit state in the bottom row, and the row is added to the bottom row when you enter.

You can also use the right-click menu to insert or delete rows in the middle of the row.

The data set is internally treated as kintone's regular table data.

### Parameters to set

Set TableSpace.

#### Table

Select which table to spread.

#### Space

Select the space in which to place the spread table.

## Limitations

If a table contains the following types of fields (columns), you cannot spread them: An error occurs when the action is executed.

-	Checkbox
-	Multi-selection
-	Attachments
-	Date and time
-	User Selection
-	Group Selection
-	Organization Selection

Because of the kintone specification, a table cannot have more than 5000 rows.
