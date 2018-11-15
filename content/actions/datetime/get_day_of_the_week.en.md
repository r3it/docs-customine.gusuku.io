---
title: Get day of the week from date
date: 2018-01-22T16:07:50+09:00
weight: 1420
---
## Summary

Gets the day of the week from a date and makes it visible to other actions.

## How to use

If you want to include the acquired day of the week in the field, select that field in the "Destination field (optional)" parameter.

Instead of putting the day of the week in the field immediately, if you want to use it in other actions, use the formula.

If you perform an action set to “Get the day of the week from date”, the day string is stored internally as the result of the action.

You can use a formula to retrieve the saved day of the week, for example, = $1.

The date field of kintone cannot be set as the day of the week will not contain any date information. It is possible to set fields such as “String (one line)”.

Example) An example of using the acquired day as another action ("[Add record](../../record/insert_record/)")

1.	Set “Get the day of the week from date”. The action number is number one.
2.	In "Mapping" of [Add record](../../record/insert_record/), put "=$1" in the date field you want to set. (If the action number for “Get the day of the week from date” is number 2, say “= $2”)

### Parameters to set

Set Date Language Format.

#### Date

Enter the date for which you want to calculate the day of the week.

If you want to refer to the value of a date or time field

```
=Date_2
```

Refer to the field code with “=” as shown in.

To calculate the day of the week for the current date, use

```
=today()
```

in the Value field.

#### Language

Specifies which language string to get the day of the week.

If the selected language is “Japanese” or “English”, it will be the specified language regardless of the login user's language setting.

If you select “Login User Language”, the user will be selected according to the language set in the profile settings of kintone. However, it does not support Chinese. The result is English day names for users who select Chinese in their profile.

#### Format

Choose whether to display the long or short format.

For Japanese long forms, the result is like Wednesday, and for short forms, the result is like Wednesday.

#### Set destination field (optional)

Specify this when setting the acquired date in another field. If you do not set it in the direct field and you want to use the result in another action, you can omit it.

## Limitations

It is not available in Chinese. If you select “Language of Login Users” as “Language”, the result will be English day names for users who select Chinese in their profile.
