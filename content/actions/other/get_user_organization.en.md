---
title: Get Belonging Organization
date: 2018-01-22T16:07:50+09:00
weight: 1620
---
## Summary

Gets the organizations to which the currently logged-in user belongs.

## How to use

When you perform this action, information about your organization is saved as a result of the action. If you belong to more than one organization, all of them will be retrieved.

You can use an expression to reference this information, for example, from $1, but you can use the [If you belong to a specified group organization](../../../conditions/condition_other_if/if_user_belongs_to) is a more typical use case.

## Limitations

If an organization has a parent-child relationship, only child organizations are retrieved if it belongs to the child organization but not the parent organization.

It cannot be retrieved if the user is a guest user.
