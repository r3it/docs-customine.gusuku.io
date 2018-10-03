---
title: Make Pulldown from Records
date: 2018-01-22T16:07:50+09:00
weight: 1800
---
## Summary

Creates a pulldown (drop-down menu) based on records retrieved by other actions.

## How to use

In preparation, the app you want to customize has a space field to place the pulldown and a field to store the pulldown values.

Create an app to define the contents of the pulldown and create a record.

In Customine customization settings, see [Retrieve all records](../../record/get_all_records/) is used to retrieve records, such as get data from the app to define the content of the pulldown.

Next, place “Create a pull-down from a record” and set the space field that you prepared, and the field that stores the pull-down values.

## Example

Suppose you have a “Product Management App” to manage your products, and you want to define a product classification in another app and select the classification code in the “Product Management App”.

1.	Create a Product Classifier Master app, place the classification code and classification name fields, and create a record.
2.	In the Manage Products app, place a field for “Product Classifier Code” and a space for the pull-down.
3.	Start customizing the Product Management App in Cutomine.
4.	When the edit screen starts,”[Retrieve all records](../../record/get_all_records/)to retrieve all records of the Product Classification Master.
5.	Place “Create pull-down from record” and set as follows:
	-	Data Storage Fields - Product Classifier Code
	-	Space - Prepositioned Space
	-	Label - > Product Classification
	-	Record - record retrieval action set in step above
	-	Fields to display - Classification Names
	-	Field that becomes a value - Classification Code  

### Parameters to set

Set Data Storage Field, Space, Label, Record, Field to Display, Field to Value.

#### Data storage fields

Select a field to store the contents of the selected pulldown.

The only field types that can be selected are String (single line).

#### Space

Select the space in which you want to display pulldowns.

#### Label

Sets the label to display in the pull-down.

#### Record

Select the action that retrieved the record for the pulldown.

In the above example, the [Retrieve all records](../../record/get_all_records/), but you can use other methods of obtaining, for example, [Retrieve records by key](../../record/get_records_by_key/) and so on.

#### Fields to Display

Specifies which fields to display in the pull-down. This field is not the field in the app you are customizing, but the field in the source app of the retrieved record.

For example, if the source app consists of “X code” and “X name”, and you want to save the “X code” as data, but you want to display “X name” on the pulldown display, so you have to choose "X name".

#### The field that will be the value

Select the field whose values you want to include in the Data Storage Field when you select it from the pull-down. This field is not the field in the app you are customizing, but the field in the source app of the retrieved record.

For example, if the source app consists of “X code” and “X name”, then “X name” is displayed on the pulldown display, but you want to save the “X code” in the “data storage field”, so you have to choose “X code".

## Limitations

-	When used on the record detail screen or record print screen, it does not drop down. The “Fields to Display” pulldown selected in the edit screen is displayed.

-	If you perform this action on the Edit Record screen or Add Record screen, the Data storage fields are no longer editable and cannot be entered directly. [Enable a field](../../field/enable_field/), but you can use theIn this case, manual entry of “data storage fields” will not be reflected on the pull-down side.

-	Smartphone version is not supported.

### Field types that can be selected as data storage fields

-	String (one line)

### Field types that can be selected as Fields to Display

-	Record Number
-	String (one line)
-	Number
-	Calculation
-	Date
-	Time
-	Date and time
-	Lookup

### Field types that can be selected as “Value Field”

-	Record Number
-	String (one line)
-	String (multiple lines)
-	Rich Editor
-	Link
-	Number
-	Calculation
-	Date
-	Time
-	Date and time
-	Lookup
