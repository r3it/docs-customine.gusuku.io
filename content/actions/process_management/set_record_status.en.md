---
title: Change Status (Specified Record)
date: 2018-01-22T16:07:50+09:00
weight: 1720
---
## Summary

Performs the specified state change action on the specified record.

## How to use

### Parameters to set

Set “Update To”, “Record”, “Change Status Action”, and “Worker Field”.

#### Destination App

Select the app whose status you want to update.

#### Record

Select the action that retrieved the record whose status you want to update.

#### Change State Action

Enter the name of the Change Status Action you have set for your app.  
(You must enter the action name, not the new status.)

#### Worker (from the destination app)

#### Worker (from this app)

If you need to set a worker for the new status, please select a field with a worker.  
(You cannot directly specify a worker.)

This parameter is optional.
You do not have to choose if you want to automatically determine the next task according to your process management settings.

When both "Worker (from update destination application)" and "Worker (from this application)" are selected, "Worker (from update application)" takes precedence and "worker (from update destination application)" is ignored.

The available fields are User Selected, Created By (of record), or Modified By (of record).

## Limitations

You cannot specify a worker directly.  
Set up a user selection field in your app and register the users you want to set up as workers.  
If there are multiple users in the Reviewer field, the first user is registered to the worker.

Alternatively, you can designate the worker who created or updated the record.
