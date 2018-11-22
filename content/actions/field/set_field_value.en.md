---
title: Set Field Value
date: 2018-01-22T16:07:50+09:00
weight: 1400
---
## Summary

Set a specified value in the field.

## How to use

### Parameters to set

Set “Field” and “Value”.

#### Field

Select a field for setting out the value.

#### Value

Set a value to be set out.

Like Excel, calculation formula could be specified by entering a text beginning with “=”.
In case when a calculation formula is specified, the calculated value will be set in the field when the action is executed.
The formula can include other field values.

Example: In the following case, “name” field value and “email” field value is separated with a space.

```
= name & " " & email
```

## Limitations

The following field type **CAN NOT** be used:

-	Space
-	Table
-	Groups
-	Calculation
-	Attachments
-	List of related records
-	Author
-	Created at
-	Modified By
-	Modified
-	Category
-	Status
-	Worker

You can also select the "String (multiple lines)" field, but you can not enter a line break with the "Value" parameter. If you want to set "value" including line feeds, use "[Set Multi Line Text Field Value](../set_multi_line_text_value)".
