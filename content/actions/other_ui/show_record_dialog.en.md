---
title: Display Record List in Dialog
date: 2018-01-22T16:07:50+09:00
weight: 1530
---
## Summary

Displays a pop-up list of records.

Users can also select records from the displayed list by radio buttons and checkboxes.

## How to use

When the action is performed, a pop-up dialog appears displaying a list of records.

When the user selects a record and presses the OK button, the action execution is complete and the selected record is set as the result of the action.

The record selected by the user, for example, [Calculate the average of a field in a record](../../aggregate/calc_records_average) to the action that receives the record.

### Parameters to set

Set “Record”, “Field to Display”, “Selection Method”, “Message Input”, “OK Button Name”, and “Cancel Button Name”.

#### Record

Specifies the action that retrieved the record to display in the list.

If you want to specify the order of records, see [Sort records](../../record/sort_records/) to sort the records, and then clickIf this parameter is set to ”[Sort records](../../record/sort_records/), and then set the action.

#### Fields to Display

Specifies the fields to display in the list.

#### Selection Method

Specifies how the user selects records.

You can choose whether to select only one record with the radio button, select multiple records with the checkbox, or disable the selection itself.

#### Message Input

Enter the text you want to display in the message portion of the dialog.

In [Show Info Dialog](../message_dialog/), you can type in the rich editor. But only normal text can be entered in this.

This parameter is optional.

#### Name of OK button

Change this parameter if you want to change the label displayed on the OK button.

#### The name of the cancel button.

If you want to change the label displayed on the Cancel button, change this parameter.

## Additional Considerations

The action is complete when the user closes the dialog by pressing OK or Cancel in the dialog. When the dialog is displayed, the action is not completed.

The action will be completed even if you press “Cancel”.

[When other actions have finished executing](../../../conditions/condition_other/when_action_complete/) and wait for this action to complete, note the above.

If you want to ignore “Cancel” and proceed to the next action only if “OK” is selected, [When other actions have finished executing](../../../conditions/condition_other/when_action_complete/) instead of [When “OK” is pressed in the confirmation/input dialog](../../../conditions/condition_other/is_confirm_dialog_ok/) condition.

## Limitations

You cannot change the order in which fields are displayed.
