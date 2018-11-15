---
title: Get Login User
date: 2018-01-22T16:07:50+09:00
weight: 1600
---
## Summary

Gets information about the currently logged-in user.

### Parameters to set

Specify "Set destination field (optional)".

#### Set destination field (optional)

Specify this option when you set the acquired user in another field. If you do not set it in the direct field and you want to use the result in another action, you can omit it.

If you set the destination to the user selection field, the other currently selected users are cleared and the login user is selected.

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
= $1.email
```

### (Example) Set the mail address of the user logged in the link field

[Display characters in spaces](../../other_ui/add_label_at_spacer), type “Text to display” as follows:

```
Welcome ${$1.name} san
```
