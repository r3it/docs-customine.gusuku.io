---
title: When Cancel Clicked in Confiramation/Input Dialog
date: 2018-01-22T16:07:50+09:00
weight: 1130
---
## Summary

Perform an action when the user cancels a confirmation or input dialog.

The action name “Cancel” is “When pressed”, but the condition is actually true if you press outside of the dialog or press the ESC key to close it.

## How to use

In order for this condition to occur, you must first go to [Show confirmation dialog](../../../actions/other_ui/confirm_dialog) or [Show input dialog](../../../actions/other_ui/input_dialog) action must be performed.

This condition fires when the appropriate dialog is displayed and the user closes anything other than “OK”.

This condition does not occur if the user chooses “OK” even though the corresponding confirmation dialog is displayed.

### Parameters to set

Set the “Confirmation/Input Dialog Action”.

#### Confirm Input Dialog Action

In which confirmation or input dialogue you clicked Cancel, To identify the dialog, use the [Show confirmation dialog](../../../actions/other_ui/confirm_dialog) or [Show input dialog](../../../actions/other_ui/input_dialog) action number.

For example, the first action displays the confirmation dialog “Do you want to save?” and the second action is “Do you want to do it?” , if number 1 is specified in the parameter of “Confirmation Dialog Result Confirmation”, the action is triggered only when “Save?” and “Do you want to print?” , it will not be activated.
