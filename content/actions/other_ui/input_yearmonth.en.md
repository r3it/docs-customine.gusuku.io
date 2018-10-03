---
title: Make Year/Month Picker
date: 2018-01-22T16:07:50+09:00
weight: 1810
---
## Summary

Create a Year/Month Selection Field.

## How to use

In preparation, the app you want to customize has a space field to place the Year/Month selection field and a date field to store the value of the selected year/month.

In Customine customization settings, place “Create Year/Month Selection Field”, and set the space fields that you prepared, and the fields where you want to store the values.

### Parameters to set

Set the Data Storage FieldSpaceLabel.

#### Data storage fields

Select a field to save the selection.

Date is the only field type available.

The selected value is saved as “the first day of the month. For example, if you select April 2018, the data storage field will be 2018-04-01.

#### Space

Select the spaces you want to display.

#### Label

Sets the label to display.

## Limitations

-	If you perform this action on the Edit Record screen or Add Record screen, the Data storage fields are no longer editable and cannot be entered directly. You can use [Enable a field](../../field/enable_field/), but in this case, manual entry of “Data Storage Fields” will not be reflected in the “Year/Month Selection” side.

-	There is no ability to deselect it.

-	Smartphone version is not supported.

### Field types that can be selected as data storage fields

-	Date
