---
title: Display Input String Dialog
date: 2018-01-22T16:07:50+09:00
weight: 1520
---
## Summary

Displays a dialog similar to the one shown. Primarily used in situations where users are prompted to enter short text.

![Input dialog](/images/ja/actions/other_ui/input_dialog/1.png)

## How to use

When the action is executed, an input dialog appears.

When the user enters text and presses the OK button, the action execution is complete and the text entered as the result of the action is set.

Expressions are used to retrieve text entered by the user.

For example, if the action that displays the input dialog is first, the [Set a value in a field](../../field/set_field_value/) in the “Value” parameter, for example,

```
=$1
```

to retrieve the input.

### Parameters to set

Set [Message input], [OK button name], [Cancel button name], and [Empty allowed].

#### Message Input

Enter the text you want to display in the message portion of the dialog.

#### Name of OK button

Change this parameter if you want to change the label displayed on the OK button.

#### The name of the cancel button.

If you want to change the label displayed on the Cancel button, change this parameter.

#### Allow Empty

If you select “Allow OK to leave empty”, you can press the “OK” button even if the input is empty.

If you select “Don't press OK if empty”, the “OK” button will not be available while the input contents are empty.

## Additional Considerations

The action is complete when the user closes the dialog by pressing OK or Cancel in the dialog. When the dialog is displayed, the action is not completed.

The action will be completed even if you press “Cancel”.

[When other actions have finished executing](../../../conditions/condition_other/when_action_complete/) and wait for this action to complete, note the above.

If you want to ignore “Cancel” and proceed to the next action only if “OK” is selected, [When other actions have finished executing](../../../conditions/condition_other/when_action_complete/) instead of [When “OK” is pressed in the confirmation/input dialog](../../../conditions/condition_other/is_confirm_dialog_ok/) condition.
