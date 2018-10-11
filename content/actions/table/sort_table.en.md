---
title: Sort Table Row
date: 2018-01-22T16:07:50+09:00
weight: 1120
---
## Summary

Sorts the rows of the table being edited by the specified field.

## How to use

### Parameters to set

Set “Table”, “Key fields (1) to (3)”, and “Sort order (1) to (3)”.

#### Table

Select the desired table.

#### Key Fields (1)

#### Key Fields (2)

#### Key Fields (3)

Select the field you want to sort by.

(1) is the highest priority, then (2) (3). In other words, values of (1) are ordered in order (2), and (3) if (1) and (2) are the same.

(2) (3) is optional.

#### Sort by (1)

#### Sort by (2)

#### Sort by (3)

Specifies whether to sort in ascending or descending order.

If the key fields (2), (3) are omitted, the sort order (2) and (3) are ignored.

## Limitations

It is not available in the record list screen. When used in the record list screen, an error is displayed when the action is executed.

You can also sort on the record details screen. However, simply changing the apparent order does not update record data.

The following fields cannot be selected as key fields:

-	Checkbox
-	Multi-selection
-	Attachments
-	User Selection
-	Organization Selection
-	Group Selection
-	Table
-	Groups

You can specify no more than three fields. Sorting on more than four fields is not supported.

### About sorting tables, including lookups

When just before saving a record like [Just before saving a record (except when deleting it)](../../../conditions/condition_event/when_record_save_exclude_delete), you cannot sorted correctly tables that contain lookups and calculated fields. It can be sorted at any other time.

This is because of the kintone specification, it is a field that cannot be modified immediately before saving.

Fields that cannot be modified just before saving are as follows:

-	Record Number
-	Author
-	Created at
-	Modified By
-	Modified
-	Status
-	Worker
-	Calculation
-	1 line of text automatically calculated
-	Attachments
-	Lookup
-	Lookup Destination Field

https://developer.cybozu.io/hc/ja/articles/202166270#step4
