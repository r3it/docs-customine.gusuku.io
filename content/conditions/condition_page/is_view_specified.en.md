---
title: If List Page is Specified View
date: 2018-01-22T16:07:50+09:00
weight: 1210
---
## Summary

Fits if the current screen is a record list screen and the name of the selected list is one of the specified names.

## How to use

This condition is used in conjunction with other “when” conditions.

For example, if you want to run it, type [When the list screen is displayed](../../condition_event/when_record_list_show), and “(All)” is specified. This means “When the list screen is displayed, the specified action will be executed if the list is (all).”

### Parameters to set

Set the List Name.

#### Name of the list

Specifies the name of the list to which the condition is to be met.

Multiple lists can be found in the **Separate by newline** can be specified. In that case, if any of them is matched, the condition is met.

If you set the list name to change in Japanese, English or Chinese, Please enter a name for each.

If you have more than one list with the same name, If you specify that name in the List Name parameter, Whichever list is displayed, the condition will be triggered.

You can also specify (worker's own) or (all).
