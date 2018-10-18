---
title: Add Record with Table Data
date: 2018-03-06T12:01:14+09:00
weight: 1020
---
## Summary

Creates a new record with table data set for the specified app.

## How to use

“Add records with table data” is an enhanced version of [Add records](../../record/insert_record).

- You cannot set values in the table with [Add records](../../record/insert_record), But when you use “Add a record with table data”, you can add a record with the default value set to the table.

-	In “Add record with table data”, you can immediately move to the edit screen of the added record.

If you don't need these features, see [Add records](../../record/insert_record) is more easier.

### Parameters to set

Specify “Append To”, “Mapping to Record”, “Table”, “Record to Table”, “Mapping to Table”, and “Screen Transition”.

#### Add to App

Select the app you want to add records to.

#### Mapping to Records

Sets the value of each field in the record to be added.

However, table values cannot be set here; table values are set in Mapping to Table later in this section.

In this mapping, the

```
= fieldCode
```

, the field code is “the field of the app being customized.”

#### Table

Select the table for which you want to set the initial value.

You cannot select more than one.

#### The underlying record for the table.

Specifies the record from which the table data is created.

#### mapping to tables

Defines the mapping that sets the data in the table.

In this mapping, the

```
= fieldCode
```

, the field code becomes the field of the table's underlying record.

#### Screen Transition

After you create a record, choose whether you want to go to the edit screen for that record.

### Example

When you want to set data in a table with “Add records with table data”, you first retrieve the record that is the source of the table data.

For example, you can create a record of another app from the editing screen of the app you are customizing, and then copy the table data from the table of the app you are customizing to the new record of another app. Consider the case.

In this example, the record from which the table data is based is the table data of the app you are customizing. So, ”[Fetch a table row as a record](../get_record_from_table) to retrieve each row of data from the table in the app you are customizing.

Next, in the Add Records With Table Data section, under the Table Source parameter, type [Fetch a table row as a record](../get_record_from_table) action.

Then, in “Mapping to Table”, you define the mapping so that values are copied from a column in the source table to the table in the target app.

## Limitations

You cannot set data for more than one table at a time.

The record will be moved to the edit screen when it is created, so if you press “Cancel” on the edit screen, the created record will remain.

If the app you are customizing differs from the kintone space of the app that creates the record, and the destination is guest space, you will get an error.

When the “Screen Transition” parameter is set to “Open the edit screen of the created record in a separate tab”, the pop-up blocker function of the browser may block the tab. In that case, please allow pop-ups in your kintone domain in your browser settings.
