---
title: Get Login User
date: 2018-01-22T16:07:50+09:00
weight: 1600
---
## Summary

Gets information about the currently logged-in user.

## How to use

This action saves the logged-in user information as a result of the action.

The logged-in user information can be referenced in parameters of other actions using an expression such as $1.name.

### What can I see?

Only list what you expect to use frequently with Customine.

-	code login name
-	name Display Name
-	Email address

Other references to this information are available in

https://developer.cybozu.io/hc/ja/articles/201942024

See Object Contents in.

## Example

In the following example, assume that you have obtained the login user with action number 1. If the action that retrieved the logged-in user is number 2, change $1 to $2.

### (Example) Set the logged-in user selection field

[Set a value in a field](../../field/set_field_value), type the Value parameter as follows:

```
= $1.code
```

### (Example) Display name (such as full name) of the user logged in as “Welcome” in a space

[Display characters in spaces](../../other_ui/add_label_at_spacer), type “Text to display” as follows:

```
Welcome ${$1.name} san
```
