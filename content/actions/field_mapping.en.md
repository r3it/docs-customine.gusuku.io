---
title: How to describe field mapping
date: 2018-01-15T17:07:50+09:00
---
## Summary

Field Mappings can be found in the[Add records](../record/insert_record/)and[Export table rows to records in another app](../record/expand_table), this parameter defines the contents of the record to be exported.

## How to Write Field Mappings

![field mapping](/images/ja/actions/field_mapping/1.png)

A screen similar to the one shown will pop up.

The right side represents the fields of records to export. The fields shown are limited to those that can set values. Fields that cannot be set, such as Record Number, are displayed.Sen.

Describe the value you want to set in “Value to set”.

### Value to set

Describes a fixed value or a value to be set by an expression.

Press the “f” button to select the field in the currently customized app and enter an expression that references the field.

Press the “a” button to select another action and enter an expression that references the result value of the action.

You can also enter expressions by hand.

Example)

-	If you want to enter a fixed string, enclose it in “”.

	```
	="2018 year"
	```

-	If you reference a field, specify the field code.

	```
	= Text_1_1
	= Number_2
	```

-	If you want to use the results of other actions, you can refer to “$ action number” or “$ action number.field code”.

	```
	= $1
	= $2.Text_1_1
	```

-	If you want to combine characters, see&” to connect it.

	```
	= "A.D. " & $1.Number & "."
	```

-	Use operators to register the results of a calculation.

	```
	= (Number_1 * Number_2) * 180 / 3.1416
	```

-	You can also use today (), now (), and format () functions.

	```
	= format(today(), 'D/M')
	```

-	If you want to select multiple values in a check box or multi-select field, clickUse.

	```
	= ['sample1', 'sample2']
	```

-	If you want to set an attachment, see[Copy attachments](../field/copy_attachment/), and specify “$ action number”.

	```
	= $1
	```

### If you want to set a blank space

If the value to be set is empty, the field will not be output instead of an empty value; for example,[Update records](../record/update_record/), it means that the value of the original field is preserved, rather than replacing the original field with a blank space.

On the other hand, if you want to set a blank space, specify the value to be set as follows:

```
=""
```

## Limitations

Values cannot be registered for the following fields:

-	A field whose value cannot be changed originally, such as a record number.
-	Attachments
-	Status
-	Category
-	Table
