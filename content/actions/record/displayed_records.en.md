---
title: Retrieve Record Displayed on List Page
date: 2018-01-22T16:07:50+09:00
weight: 1730
---
## Summary

Retrieves the records displayed on the current page in the list screen.

## How to use

Retrieved records can be retrieved, for example, [Calculate the average of a field in a record](../../aggregate/calc_records_average), or it can be aggregated by an aggregate function or you can use equations to make calculations.

### Parameters to set

There are no parameters.

## Limitations

It cannot be used on the smartphone screen.

If the list spans more than one page, only records for the currently displayed page are retrieved. Records on pages that are not visible are not retrieved.

If you want to retrieve all records that are not visible, you can use [Fetch all records by criteria in a list](../get_record_using_list).
