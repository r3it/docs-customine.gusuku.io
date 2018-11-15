---
title: Get Belonging Group
date: 2018-01-22T16:07:50+09:00
weight: 1610
---

## Summary

Gets the group (role) to which the currently logged in user belongs.

## How to use

When this action is executed, the information of the group to which it belongs is saved as the result of the action.

It is also possible to refer to this information from $1 etc using an expression.
But more typical usage is to combine it with [belonging to a designated group / organization](../../../conditions/condition_other_if/if_user_belongs_to/).

### Parameters to set

Specify "Set destination field (optional)".

#### Set destination field (optional)

Specify this when you want to set the acquired group to another field. If you do not set it in the direct field and you want to use the result in another action, you can omit it.

If you set the set destination to the group selection field, the other group currently selected is cleared and the group to which the logged-in user belongs is selected. If it belongs to more than one group, it will be set.

If you set the destination to a character string (1 line) etc., the group name will be set. If belonging to more than one group, the group names are arranged in comma-delimited order.

## Limitations

It can not be acquired if the user is a guest user.
