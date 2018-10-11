---
title: Display Confirmation Dialog
date: 2018-01-22T16:07:50+09:00
weight: 1515
---
## Summary

Displays a dialog similar to the one shown. Mainly used when asking for confirmation from the user.

![Confirm dialog](/images/ja/actions/other_ui/confirm_dialog/1.png)

## How to use

### Parameters to set

Set [Message input], [OK button name] and [Cancel button name].

#### Message Input

Enter the text you want to display in the message portion of the dialog.

#### Name of OK button

Change this parameter if you want to change the label displayed on the OK button.

#### The name of the cancel button.

If you want to change the label displayed on the Cancel button, change this parameter.

## Additional Considerations

The action is complete when the user closes the dialog by pressing OK or Cancel in the dialog. When the dialog is displayed, the action is not completed.

The action will be completed even if you press “Cancel”.

[When other actions have finished executing](../../../conditions/condition_other/when_action_complete/) and wait for this action to complete, note the above.

If you want to ignore “Cancel” and proceed to the next action only if “OK” is selected, [When other actions have finished executing](../../../conditions/condition_other/when_action_complete/) instead of [When “OK” is pressed in the confirmation/input dialog](../../../conditions/condition_other/is_confirm_dialog_ok/) condition.
