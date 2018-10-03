---
title: If Field is NOT Accessible to Show
date: 2018-01-22T16:07:50+09:00
weight: 1140
---
## Summary

This condition is true if the currently logged in user is not able to view the specified field.

“Viewable” means that field access in the app does not restrict field viewing.

## How to use

In advance, set the access rights of the field in the kintone standard app settings screen.

### Parameters to set

Set the Fields.

#### field

Select the fields you want to check.

If multiple selections are made, the condition is met if all of the selected fields are not viewable. If at least one field is visible, the condition will not be met.

## Precautions

In this case, “Not visible” means that you do not have “View” access to the field.“”[Hide a field or group](../../../actions/field/hide_field/)is different from making the field visually invisible.

Even if it is not visible on the screen with “Hide Fields and Groups”, it will be judged as viewable if you have access to “View”.

## Limitations

The following fields are not selectable:

-	Table
-	Groups
-	Attachments
-	List of related records
