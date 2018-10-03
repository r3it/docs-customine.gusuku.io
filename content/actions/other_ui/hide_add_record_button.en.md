---
title: Hide Add Record Button
date: 2018-01-22T16:07:50+09:00
weight: 1720
---
## Summary

Hides the Add Record button (plus icon) on the record list screen or record detail screen.

## How to use

Condition [When the details screen is displayed](../../../conditions/condition_event/when_record_detail_show/) to hide the add record button, as shown in the following figure, the icon in the red frame is hidden.

![Hide Add Record Button](/images/ja/actions/other_ui/hide_add_record_button/1.png)

Likewise, see [When the list screen is displayed](../../../conditions/condition_event/when_record_list_show/) to hide the add record button  and disappears from the list screen.

If you want to remove the Add Record button from both the detail screen and the list screen, you need to set up two actions and “Hide Record Add Button” on each screen.

[Hide Record Reuse Button](../hide_reuse_record_button/) at the same time.

### Parameters to set

There are no parameters.

## Limitations

It does not disable the Add Record screen itself. If you turn off the icon in this “What to do”, you can still display the Add Record screen using keyboard shortcuts and other methods.

Smartphone version screen is not supported. Using this “do” on the smartphone version has no effect and does not result in an error.

There is no “to do” to re-display the Add Record button that has been erased.
