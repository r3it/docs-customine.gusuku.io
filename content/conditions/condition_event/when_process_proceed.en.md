---
title: When Process Action Proceeded
date: 2018-01-22T16:07:50+09:00
weight: 1078
---
## Summary

Executes a Customine action when a process management action is performed.

## How to use

A condition that you set when you want the Customine action to be executed when the user performs a process management action on the record details screen.

After setting this condition, set the “What to do” to” [Set a value in a field](../../../actions/field/set_field_value/) to change the value of a field, such asYou can perform customizations such as “Changing the value of a field when a process management action is performed.”

### Parameters to set

Specify Process Management ActionPre-Change Process Management StatusPost-Change Process Management Status.

All of these are optional, so you don't have to specify them. In that case, this condition is triggered if the process management action is performed in any action or state, regardless of the action or state.

#### Process Management Actions

Select which action to trigger the condition.

If more than one action is selected, one of the selected actions will be executed.

If none is specified, any action is OK.

#### Pre-Change Process Management Status

Select a status if you want the condition to fire only if the state at the time the action was taken is a certain value.

If multiple statuses are selected, any one of the selected statuses matches will be OK.

For example, if you select Unprocessed and Processing for this parameter, an action that transitions from Unprocessed to Processing or In Progress to Completed will trigger a condition. Actions that transition from Completed to Processing do not trigger conditions.

#### Post-Change Process Management Status

Select a status if you want the condition to fire only if the status after you perform the action is a certain value.

If multiple statuses are selected, any one of the selected statuses matches will be OK.

For example, if you select “Complete” for this parameter, an action that transitions from “In Process to Complete” will trigger a condition. Actions that transition from Completed to Processing do not trigger conditions.
