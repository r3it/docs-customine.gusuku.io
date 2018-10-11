---
title: Change Status (Current Record)
date: 2018-01-22T16:07:50+09:00
weight: 1710
---
## Summary

Executes the specified state change action for the current record.

## How to use

### Parameters to set

Set the Change State ActionReviewer Field.

#### Change State Action

Enter the name of the Change Status Action you have set for your app.  
(You must enter the action name, not the new status.)

#### Reviewer Field

If you need to set a worker for the new status, use the  
Please select a field with a worker.  
(You cannot directly specify a worker.)

The available fields are User Selected, Created By (of record), or Modified By (of record).

## Limitations

You cannot specify a worker directly.  
Set up a user selection field in your app and register the users you want to set up as workers.  
If there are multiple users in the Reviewer field, the first user is registered to the worker.

Alternatively, you can designate the worker who created or updated the record.
