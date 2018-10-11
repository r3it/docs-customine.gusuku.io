---
title: Remove Duplicated Records
date: 2018-03-06T12:01:14+09:00
weight: 1800
---
## Summary

Excludes records with duplicate values from the specified key.

## How to use

You must prepare records with [Retrieve all records](../get_all_records) or [Retrieve records by key](../get_records_by_key), and so on.

If records has duplicate record, the one that goes down in the order is deleted.

### Parameters to set

Set the Record Selection Action and Key Field.

#### Record Selection Actions

Select the action that retrieved the record of interest.

You can't choose yourself.

#### Key Fields

Select the fields that you want to compare when determining whether records are duplicates.

For example, if you specify the City field, and there are more than one record for the same state, the second and subsequent records are deleted, leaving only the first one.

You can select multiple fields. In that case, Access finds duplicate records that match all the selected fields.

You can select the following types of fields:

-	String (one line)
-	Number
-	Calculation
-	Date and time
-	Date
-	Time
-	Lookup
-	Radio buttons
-	Drop-down
-	Link
