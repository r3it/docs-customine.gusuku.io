---
title: If the Login User is Specified One
date: 2018-03-26T14:53:50+09:00
weight: 1010
---
## Summary

The condition is met if the user accessing the app is a designated user.

## How to use

This condition is used in conjunction with other “when” conditions.

For example, if you want to specify the condition “When the list screen is displayed and the current user is the specified user” when the list screen is displayed, Combine this condition with “When the list screen is displayed”.

### Parameters to set

Specify the Login Name.

#### Login name

Specifies the user's login name. Not a display name.

You can specify more than one user by using a single string. In that case, the condition is met if it matches one of the specified users. For example, if you specify “A, B, C”, it is OK if the login user is A, B, or C, and NG if the login user is D.
