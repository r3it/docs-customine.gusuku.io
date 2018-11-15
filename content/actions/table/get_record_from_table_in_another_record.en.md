---
title: Retrieve Subtable Row in another Record as Record
date: 2018-03-06T12:01:14+09:00
weight: 1005
---
## Summary

Retrieves table rows contained in other records so that you can manipulate them as if they were records.

## How to use

This is similar to [Fetch a table row as a record](../get_record_from_table), but “Fetch a table row as a record” retrieves from the record that the user has opened in the record edit screen, detail screen, etc. whereas “Fetch a table in another record as a record” to get from records fetched by other action.

Once retrieved, you can use the rows as you would any other “DO” record.

For example, [Export Records](../../record/write_record) to export to other apps, or to [Remove duplicates from records](../../record/remove_duplicated_records) to remove duplicate rows and connect them to other “DO”.

### Parameters to set

Set “Record containing table” “Table” “Whether to get empty rows”.

#### Records containing tables

Specify which record to retrieve. Select the action that retrieved the record.

If the record selection action selected here does not retrieve any rows, no error occurs, and the retrieval result of “Fetch tables in other records as records” is empty (no rows).

Conversely, if a record contains more than one row, the table is retrieved from only the record in the first row of the record, not from the records in the second row.

#### Table

Select which table you want to retrieve from.

#### Whether to get empty rows

Select Suppress Empty Rows to not retrieve rows that are empty in table rows.

In this case, “empty rows” means “all columns (fields) are empty and unselected”. Note that if a field has an initial value, it is not considered empty if it is left in the field. Also, if there are fields that cannot be unselected, such as radio buttons, they cannot be empty and will always be exported.
