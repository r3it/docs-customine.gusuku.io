---
title: If the Login User do NOT Belongs to Group/Organization
date: 2018-03-26T14:53:50+09:00
weight: 1015
---
## Summary

Determines whether the currently logged-in user **not** belongs to the specified group or organization.

## How to use

This condition is used in conjunction with other “when” conditions.

For example, if you want to specify a condition that “When the list screen is displayed and the current user does not belong to Organization A” when the list screen is displayed,Combine this condition with “When the list screen is displayed”.

### Parameters to set

Specify the Group/Organization to which the user belongs Group Code/Organization Code.

#### The group/organization to which the user belongs

If you want to determine a group, see [Get the group (role) in which you belong](../../../actions/other/get_user_roles) to specify the action in which you installed.

If you want to determine your organization, see [Get your organization](../../../actions/other/get_user_organization) to specify the action in which you installed.

#### Group Code/Organization Code

Enter the Group Code or Organization Code.

## Limitations

If the organization has a parent-child relationship, and you specify a parent organization for Group Code/Organization Code, and the user does not belong directly to the parent organization, the system determines not affiliated.
