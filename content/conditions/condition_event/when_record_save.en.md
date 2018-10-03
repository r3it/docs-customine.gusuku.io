---
title: when the record is saving include deleting
date: 2018-01-22T16:07:50+09:00
weight: 1050
---
## Summary

Performs an action immediately before you save or delete a record.

## How to use

Specify the condition to perform the action if one of the following occurs:

-	When a user presses the Save button on the Add or Edit screen of a record.
-	When you press the pencil button to edit a record inline in the list screen, and then press the Save button.
-	When the user selects the Delete Record menu on the record details screen
-	When a user presses the delete button “✖” on the record list screen.

It is just before saving, so you can cancel the save by performing a specific action with this condition. Specifically, you can perform an action that causes an error in a field, or you can use [Cancel saving records](../../../actions/other/cancel_submit), records are not saved and remain in the edit screen.

※*You cannot cancel the deletion by causing an error in the field.*

## Limitations

It does not activate if you delete it from the smartphone screen.

Both save and delete are activated only from the kintone standard screen operation. [Update records](../../../actions/record/update_record/), when a record is saved using customization, it is not activated.

### To rewrite the value of a field:

If you combine the action of rewriting the value of a field during this condition, the following fields will not be reflected when you set the value:

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

This is a limitation by the kintone specification.

https://developer.cybozu.io/hc/ja/articles/202166270#step4
