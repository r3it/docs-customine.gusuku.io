---
title: If Field Contains Two or More Value
date: 2018-01-22T16:07:50+09:00
weight: 1120
---
## Summary

A field that can be multi-selected, satisfies the condition if there are actually multiple selections.

## How to use

### Parameters to set

Set the Fields.

#### field

Select the fields you want to check.

## Limitations

You can only select one of the following types of fields:

-	Checkbox
-	Multi-selection
-	Attachments
-	User Selection
-	Group Selection
-	Organization Selection
-	Worker
-	Table

Attachment fields (which are columns) in a table are not supported on the record edit screen and add screen.In this case, it is always considered “Not satisfied” regardless of the actual number of attachments.

Attachment fields are also correctly determined if they are outside the table.
