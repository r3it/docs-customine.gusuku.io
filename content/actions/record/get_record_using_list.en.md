---
title: Retrieve All Record by List Page Condition
date: 2018-01-22T16:07:50+09:00
weight: 1735
---
## Summary

Retrieves records for all pages in the search criteria of the currently displayed list in the list screen.

## How to use

For similar [Retrieve the record displayed on the screen in a list](../displayed_records) is available. When the number of records is large, and the difference comes out when it does not fit on one page.
“Retrieve records displayed on screen in list” can only be retrieved for the page displayed on the screen. But this can be retrieved even for pages that are not displayed on the screen.

Retrieved records can be retrieved, for example, [Calculate the average of a field in a record](../../aggregate/calc_records_average), or it can be aggregated by an aggregate function or you can use equations to make calculations.

### Parameters to set

There are no parameters.

## Limitations

Categories are not supported for apps that use the category. Even if the user selects a category to narrow the list, the Records for all categories are retrieved.

If the number of records is very large, it may take a very long time to retrieve all the records.
