---
title: Set Error at Field
date: 2018-01-22T16:07:50+09:00
weight: 1250
---
## Summary

Displays the error in the field.

Combined with the condition [If the field value is a specific value](../../../conditions/condition_field/field_value_condition), it can be used for more complex error checking.

## How to use

If you want to check for errors based on a combination of values in several fields, you can use this and the ”[If the field value is a specific value](../../../conditions/condition_field/field_value_condition)“.

If you just want to see an error when you're on the screen, see [When an additional screen is displayed](../../../conditions/condition_event/when_record_create_show) and other screen display conditions.

### Parameters to set

Set FieldError Message.

#### field

Select which field represents an error.

#### Error message

Enter the error message to display if there are errors.

## Limitations

The following field type **CAN NOT** be used:

-	Table
-	Space
-	Groups
-	List of related records

You cannot specify a field in a table and a field outside the table at the same time, or a field in a different table at the same time. If you want to check fields in and out of a table or in different tables at once, you can separate them into multiple actions.
