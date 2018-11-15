---
title: Copy Attachment
date: 2018-01-22T16:07:50+09:00
weight: 1600
---
## Summary

Copy the attachment.

## How to use

When you do this, you copy the attachment and temporarily save it to kintone. It uses kintone's “disk use”. In this situation, it has not been set to any field.

If more than one file is attached in the selected attachment field, all files will be copied.

The copied attachments can be found in the [Add records](../../record/insert_record/) field mapping can be set to a field in another record.

Example: Create a new record and set the copied attachment to the field in that record

1.	Assume that you set up “Copy Attachments” and the action number is number 1.
2.	Use [Add records](../../record/insert_record/), enter “= $1” for the attachment field you want to set to (If the action number for “Copy Attachments” is number 2, then “= $2”).

### Parameters to set

Set the Source Attachment Field.

#### Source Attachment Field

Select the attachment field you want to copy from.

## Limitations

If the user added an attachment in the Add Record or Edit screen and has not yet been saved, the added file cannot be copied. Only saved files can be copied.

You cannot select a field that is a column in a table.
