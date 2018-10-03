---
title: Clear All Fields
date: 2018-01-22T16:07:50+09:00
weight: 1420
---
## Summary

Clears the specified field.

## How to use

### Parameters to set

Set the Exclude Fields.

#### Exclude Fields

Select the fields you do not want to clear. You can select more than one field.If no selection is made, all fields that can be cleared are cleared.

Built-in fields, such as record numbers, are not cleared.

If there is a table to clear, all rows in that table are deleted.

Special behavior occurs when the selected field is a field (column) in the table. In this case, columns other than the specified field **in that table** are cleared. Fields outside the table are not cleared.

## Limitations

Not available in the list screen.

The following fields will not be cleared:

-	Record Number
-	Author
-	Created at
-	Modified By
-	Modified
-	Category
-	Status
-	Worker
