---
title: Write Table Row to Another App as Record
date: 2018-01-22T16:07:50+09:00
weight: 1780
---
## Summary

Export the data from the table in the customized app as a record to another app.

## How to use

### Parameters to set

Set “Source Table” “Destination App” “Mapping” “Whether to export empty rows”.

#### Source Table

Select the table field from which you want to export data.

#### Export to

Select the app you want to export to.

#### Mapping

Define the data to export.

For more information on how to write this parameter, see [How to Write Field Mappings](../../field_mapping/) for more information.

When you reference a field in Value to Set, you can reference a field in the Source Table.

#### Whether to export empty rows

If you select Don't Export Empty Rows, **If the original table row is** empty, no records are exported for that row.

It is based on whether the source table row is empty, not whether the destination record is empty.

In this case, “empty rows” means “all columns (fields) are empty and unselected”. Note that if a field has an initial value, it is not considered empty if it is left in the field.Also, if there are fields that cannot be unselected, such as radio buttons, they cannot be empty and will always be exported.

Even if it is set to “Don't write empty rows”, depending on the mapping settings, theRecords with no data remain likely to be exported.
