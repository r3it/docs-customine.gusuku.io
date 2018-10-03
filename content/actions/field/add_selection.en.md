---
title: Add Selection to Field
date: 2018-01-22T16:07:50+09:00
weight: 1425
---
## Summary

Add a selection in a field of type that allows you to select more than one choice.

## How to use

For example, if the field is checked, theLet's assume you have four choices: Breakfast, Lunch, Dinner, and Evening.

If Value is set to Breakfast, then breakfast is set when the action is performed.

When this is the case, the original selection is retained.For example, if “Evening” is selected and “Breakfast” is set, the two will be selected: “Breakfast” and “Evening”.

If you try to do the same with [Set a value in a field](../set_field_value/) 
The selection of "Evening" which was originally selected was canceled and only "Breakfast" was set.

### Parameters to set

Set FieldValue.

#### field

Select the field you want to set to.

#### Value

Specifies the value to select.

You can also select multiple values using an expression such as the following:

```
=["Breakfast", "Lunch"]
```

## Precautions

It does not mean adding a choice.

For example, if the option set to the checkbox in the app settings is two types of “A” and “B”, if you try to add “C” with this action, it does not mean that the choices increase to "A" "B" "C".

If you try to do this, kintone displays an error.

## Limitations

The fields you can select are of the following types:

-	Checkbox
-	Multi-selection
-	User Selection
-	Group Selection
-	Organization Selection
