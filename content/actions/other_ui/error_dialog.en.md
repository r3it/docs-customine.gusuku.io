---
title: Display Error Dialog
date: 2018-01-22T16:07:50+09:00
weight: 1505
---
## Summary

Displays a dialog similar to the one shown. Mainly used to display critical error messages to the user.

![Error dialog](/images/ja/actions/other_ui/error_dialog/1.png)

## How to use

### Parameters to set

Set Message Input and OK Button Name.

#### Message Input

Enter the text you want to display in the message portion of the dialog.

#### Name of OK button

Change this parameter if you want to change the label displayed on the OK button.

## Additional Considerations (1)

The action is complete when the user closes the dialog by pressing OK in the dialog. When the dialog is displayed, the action is not completed.

[When other actions have finished executing](../../../conditions/condition_other/when_action_complete/) and wait for this action to complete, note the above.

## Additional Considerations (2)

The original record saving and process management actions are not canceled even if you execute "Display error dialog" under the condition of "[just before saving / deleting record](../../../conditions/condition_event/when_record_save/)" or "[when executing action of process management](../../../conditions/condition_event/when_process_proceed/)".

If you want to cancel the record save or process management action by error, use "[Set error in record](../../error_check/set_record_error/)".
