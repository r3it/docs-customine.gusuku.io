---
title: Sort Records
date: 2018-03-06T12:01:14+09:00
weight: 1810
---
## Summary

Sorts records by the specified field.

## How to use

You must prepare records with [Retrieve all records](../get_all_records) or [Retrieve records by key](../get_records_by_key), and so on.

### Parameters to set

Set the Record Selection Action, Key Fields (1) to (3), and Sort Order (1) to (3).

#### Record Selection Actions

Select the action that retrieved the record of interest.

You can't choose yourself.

#### Key Fields (1)

#### Key Fields (2)

#### Key Fields (3)

Select the field you want to sort by.

(1) is the highest priority, then (2) (3).In other words, values of (1) are ordered in order (2), and (3) if (1) and (2) are the same.

(2) (3) is optional.

#### Sort by (1)

#### Sort by (2)

#### Sort by (3)

Specifies whether to sort in ascending or descending order.

If the key fields (2), (3) are omitted, the sort order (2) and (3) are ignored.

## Limitations

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
