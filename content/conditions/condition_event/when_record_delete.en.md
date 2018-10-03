---
title: when the record is deleting
date: 2018-01-22T16:07:50+09:00
weight: 1055
---
## Summary

Performs an action just before deleting a record.

## How to use

Specify the condition to perform the action if one of the following occurs:

-	When the user selects the Delete Record menu on the record details screen
-	When a user presses the delete button “✖” on the record list screen.

Since it was just before you deleted it, see [Cancel saving records](../../../actions/other/cancel_submit) to cancel the deletion.

Please refer to [Just before saving a record (except when deleting it)](../when_record_save_exclude_delete/), you cannot cancel by setting an error in a field.

## Limitations

It does not activate if you delete it from the smartphone screen.

kintone only works when removing from standard screen operations. It does not fire if you delete a record using customization.
