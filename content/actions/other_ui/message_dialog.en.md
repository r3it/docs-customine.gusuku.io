---
title: Display Information Dialog
date: 2018-01-22T16:07:50+09:00
weight: 1500
---
## Summary

Displays a dialog similar to the one shown.Used primarily for the purpose of displaying information to the user.

![情報ダイアログ](/images/ja/actions/other_ui/message_dialog/1.png)

## How to use

### Parameters to set

Set Message Input and OK Button Name.

#### Message Input

Enter the text you want to display in the message portion of the dialog.

#### Name of OK button

Change this parameter if you want to change the label displayed on the OK button.

## Additional Considerations

The action is complete when the user closes the dialog by pressing OK in the dialog. When the dialog is displayed, the action is not completed.

[When other actions have finished executing](../../../conditions/condition_other/when_action_complete/) and wait for this action to complete, note the above.
