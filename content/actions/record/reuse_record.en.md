---
title: レコードを再利用する
date: 2018-03-06T12:01:14+09:00
weight: 1820
---
## Summary

You will be taken to the screen to reuse records.

## How to use

### Parameters to set

Set the Record.

#### Record

Specifies the action that retrieves the records you want to reuse.

This setting is optional. If omitted, the record currently displayed in the record detail screen or record edit screen will be reused.

If the current screen is a list screen or an append record screen, omitting this parameter causes an error when executing the action.In the list screen, if you specify a record without omitting it, no error occurs.

## Limitations

You cannot move to the reuse screen of other apps. If you specify a record from another app as “Record”, the destination will be a record with the same record number in the current app.
