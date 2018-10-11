---
title: When OK Clicked in Confiramation/Input Dialog
date: 2018-01-22T16:07:50+09:00
weight: 1130
---
## Summary

Perform the action when the user presses OK in a confirmation or input dialog.

## How to use

In order for this condition to occur, you must first go to [Show confirmation dialog](../../../actions/other_ui/confirm_dialog) or [Show input dialog](../../../actions/other_ui/input_dialog) action must be performed.

This condition fires when the appropriate dialog is displayed and the user presses OK.

This condition does not occur if the user chooses Cancel even though the appropriate confirmation dialog is displayed.

### Parameters to set

Set the “Confirmation/Input Dialog Action”.

#### Confirm Input Dialog Action

In which confirmation or input dialogue you press OK, clickTo identify the dialog, use the[Show confirmation dialog](../../../actions/other_ui/confirm_dialog) or [Show input dialog](../../../actions/other_ui/input_dialog) action number.

For example, the first action displays the confirmation dialog “Do you want to save?” and the second action is “Do you want to do it?” , if number 1 is specified in the parameter of “Confirmation Dialog Result Confirmation”, the action is triggered only when “Save?” and “Do you want to print?” , it will not be activated.
