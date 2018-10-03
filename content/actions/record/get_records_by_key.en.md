---
title: キーを指定してレコードを取得する
date: 2018-01-22T16:07:50+09:00
weight: 1710
---
## Summary

Retrieves a record with the specified key from the specified app.  
The retrieved records can be used in other actions.

## How to use

### Parameters to set

Set “Get from app”, “Key field”, and “Key value”.

#### Get it from

Select the app for which you want to retrieve records.

#### Key Fields

Select the field you want to use to retrieve records from.  
You cannot select a field in a table.

#### Key Value

Enter the key value of the record you want to retrieve.

## Limitations

As of version 1.14, the following field types cannot be selected as “key fields”:

-	Multi-selection
-	Checkbox
-	Attachments
-	User Selection
-	Group Selection
-	Organization Selection

There are currently no improvements to make them selectable.

If you want to retrieve records based on these fields, use [Retrieve records by specifying criteria](../get_records_by_query).
