---
title: Put Simple Search Form on List Page
date: 2018-01-22T16:07:50+09:00
weight: 1755
---
## Summary

Set up a search form to search for “= (equals)” in one field on the list screen.

## How to use

When you execute “Set up a simple search form on the list screen”, the search form is displayed on the list screen. Users enter search criteria in this search form and press the “Search” button to further refine the list of records displayed on the list screen.

If the “List” of the currently selected kintone is filtered by the user, Searches for “List” and the conditions that the user entered in the search form are concatenated with “And (AND)”. In other words, it will be further filtered from the criteria in the “List”.

[Set up a search form to search by keyword on the list screen](../create_search_form) the main differences between are as follows:

-	You can only select one field for the condition.
-	“= (equals)” instead of keyword search.
-	The form will appear next to the menu.

![Search form](/images/ja/actions/other_ui/create_search_form_eq/1.png)

### Parameters to set

Set the Search Criteria Field.

#### Search criteria field

Select one of the fields that you want to appear in the search form as search criteria.

The table below shows which field types can be selected, what type of input they will be on the search form, and what search criteria will be.

| Field Type        | Search Criteria Entry Form | Search Criteria Type |
|-------------------|----------------------------|----------------------|
| String (one line) | String Input               | = (equal to)         |
| Link              | String Input               | = (equal to)         |
| Number            | String Input               | = (equal to)         |
| Calculation       | String Input               | = (equal to)         |

## Limitations

As shown in the previous table, the search criteria are determined by the field type. You cannot search by any other criteria. For example, in the case of “String (one line)”, it is always “= (equal)” and cannot be searched with “contains”.

Smartphone app is not supported. When running in the smartphone app, no error occurs, but no form is displayed.

You cannot have more than one simple search form. [Set up a search form to search by keyword on the list screen](../create_search_form) and “Install a simple search form on the list screen” at the same time.

If there is a duplicate list name in the app list settings, “The list was not available to get or to change. List “XXXX” has a duplicate name. Please change the name to a unique name.” error will appear.
