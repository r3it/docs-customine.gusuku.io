---
title: Put Keyword Search Form on List Page
date: 2018-01-22T16:07:50+09:00
weight: 1750
---
## Summary

Set up a search form to search mainly by keyword on the list screen.

However, search for numeric and calculated fields by “= (equals)” instead of keywords.

## How to use

When you execute “Set up a search form to search by keyword on the list screen”, the search form is displayed on the list screen.Users enter search criteria in this search form and press the “Search” button to further refine the list of records displayed on the list screen.

If you set up multiple fields as criteria and enter criteria for each field, You can search for these conditions by concatenating them with “and (AND)”.

If the “List” of the currently selected kintone is filtered by the user, Searches for “List” and the conditions that the user entered in the search form are concatenated with “And (AND)”. In other words, it will be further filtered from the criteria in the “List”.

[Set up a simple search form on the list screen](../create_search_form_eq) the main differences between are as follows:

-	You can select multiple criteria fields.
-	The search criteria for “String (one line)” will be a keyword search instead of “= (equal)”.
-	The form will appear at the bottom of the menu.

![Search form](/images/ja/actions/other_ui/create_search_form/1.png)

### Parameters to set

Set the Search Criteria Field.

#### Search criteria field

Select the fields you want to appear in the search form as search criteria.

The table below shows which field types can be selected, what type of input they will be on the search form, and what search criteria will be.

| Field Type              | Search Criteria Entry Form | Search Criteria Type                        |
|-------------------------|----------------------------|---------------------------------------------|
| String (one line)       | String Input               | (keywords entered as search criteria)       |
| Lookup                  | String Input               | (keywords entered as search criteria)       |
| Link                    | String Input               | (keywords entered as search criteria)       |
| Number                  | String Input               | = (equal to)                                |
| Calculation             | String Input               | = (equal to)                                |
| String (multiple lines) | String Input               | (keywords entered as search criteria)       |
| Rich Editor             | String Input               | (keywords entered as search criteria)       |
| Checkbox                | Drop-down                  | Include (selected items as search criteria) |
| Radio buttons           | Drop-down                  | Include (selected items as search criteria) |
| Drop-down               | Drop-down                  | Include (selected items as search criteria) |
| Multi-selection         | Drop-down                  | Include (selected items as search criteria) |
| Date         | Two String Input              | (check below.) |

The search condition of the date is as follows.

- The condition when inputting only the left side is "date >= left input condition"
- The condition for inputting only on the right side is "date <= right input condition"
- When both are entered, "date >= left input condition AND date <= right input condition"


## Limitations

You cannot change the order in which fields appear in the search form.

You cannot search for more than one field by “or (OR)”.

As shown in the previous table, the search criteria are determined by the field type. You cannot search by any other criteria.For example, in the case of “string (one line)”, it is always “contains” and cannot be searched by “= (equal)”.

Smartphone app is not supported. When running in the smartphone app, no error occurs, but no form is displayed.

You cannot have more than one search form. [Set up a simple search form on the list screen](../create_search_form_eq) and “Set up a search form to search for keywords on the list screen”.

If there is a duplicate list name in the app list settings, “The list was not available to get or to change. List “XXXX” has a duplicate name. Please change the name to a unique name.” error will appear.

When entering the search condition of the date field, it is necessary to specify the date specification with a hyphen delimiter like "2018-11-05". If you enter it with a separator as in other formats, for example, "2018/11/5", you get an error "Date format is invalid" when searching. As of version 1.30, you need to type in characters, but we plan to improve it so that we can choose from the calendar in the future.
