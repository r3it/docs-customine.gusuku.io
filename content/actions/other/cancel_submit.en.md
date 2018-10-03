---
title: Cancel Save of Record
date: 2018-01-22T16:07:50+09:00
weight: 1700
---
## Summary

Cancels the record save process, such as “just before saving a record.” “After Save” cannot be canceled.

## How to use

Place this action if you want to perform some actions starting at the condition “just before saving a record” and cancel saving for a particular condition.

A typical example would be to issue a confirmation dialog on save and cancel the save of the record when the user presses the Cancel button, as shown below.

1.	Show confirmation dialog for “About to save a record”
2.	“Cancel saving of record” when pressing “Cancel” in the confirmation/input dialog

This is **Cancel save of record**, but the addition to “just before saving a record,” you can cancel “When performing a process management action”.

## Limitations

“Immediately after saving a record” is already after the record has been saved, so you cannot cancel (revert to before saving) a save with Cancel Save Record.
