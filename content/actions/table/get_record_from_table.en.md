---
title: Retrieve Subtable Row as Record
date: 2018-03-06T12:01:14+09:00
weight: 1000
---
## Summary

Retrieves a table row so that you can manipulate it like a record.

## How to use

Retrieves each row from the table of records that the user has opened in the record edit screen, detail screen, etc.Once retrieved, you can use the rows as you would any other “do” record.

For example, [Export Records](../../record/write_record) to export to other apps, or you can also connect to [Remove duplicates from records](../../record/remove_duplicated_records).

### Parameters to set

Table Set whether to get empty rows.

#### Table

Select which table you want to retrieve from.

#### Whether to get empty rows

Select Suppress Empty Rows to not retrieve rows that are empty in table rows.

In this case, empty rows means all columns (fields) are empty and unselected.
Note that if a field has an initial value, it is not considered empty if it is left in the field.
Also, if there are fields that cannot be unselected, such as radio buttons, they cannot be empty and will always be exported.
