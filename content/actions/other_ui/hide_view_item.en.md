---
title: Remove Choice from List Page
date: 2018-01-22T16:07:50+09:00
weight: 1780
---
## Summary

Removes the specified option from the list choice (pull-down item) on the list screen.

## How to use

The main condition is [When the list screen is displayed](../../../conditions/condition_event/when_record_list_show/), specify additional conditions to prevent certain list choices from disappearing during that condition.

For example, an additional condition would be [If the logged-in user is a guest,](../../../conditions/condition_other_if/user_is_guest_condition/) can be combined with, you can remove list settings that you do not want to show to guest users from the pull-down.

### Parameters to set

Set the List Name.

#### Name of the list

Specify the name of the “List” that you want to erase. You can also delete multiple “list” at once. In that case, enter the names you want to delete on a line by line break.

If you change the name of the list for each language, specify the name of each language separated by a carriage return.

Specifying a name for a “list” that does not exist does not result in an error.

## Limitations

You cannot prevent the list of deleted settings by simply disappearing the drop-down selection on the screen. The pull-down selection will disappear, but if the user knows the link URL to the list, they will still be able to view it from there.

For the same reason, if the selection at the top of the list disappears, but the screen transitions from “Link to App”, The list is displayed with the selection that was at the top before it was removed.

Smartphone version screen is not supported. It does not cause an error even if you run it on the smartphone version.
