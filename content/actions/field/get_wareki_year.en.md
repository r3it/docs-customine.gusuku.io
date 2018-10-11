---
title: Convert Christian Calendar to Japanese
date: 2018-01-22T16:07:50+09:00
weight: 1540
---
## Summary

Converts a string or date field into a Japanese calendar and sets it to another field.

## How to use

### Parameters to set

Specify the “Convert From Date”, “Set Gengo to” and “Set Japanese calendar years to”.

#### Source Date

Select the field with the date recorded in the year.

You can choose from the following field types:

-	String (one line)
-	Date
-	Date and time
-	Created at
-	Modified

If you choose a single-line string field, the value must be set in the correct date format.

#### The name of the era is set to

Select the field for which you want to set the era name.

Only strings (one line) can be selected.

#### Japanese year set to

Select the field for which you want to set Japanese year numbers.

You can select a string (single line) or a numeric field.

The first year of the era name is “1” instead of “1”.

## Limitations

### Corresponding Era Range

To determine which era supports era era era era, see the user's browser (*).

\(*) It depends on the browser from which the user accesses the customized kintone app, not the browser used to create customizations in Customine.

- IE11 ... After Meiji(A.D. 1873)
- Chrome ... After Taika(A.D. 645)
- FireFox ... After Taika(A.D. 645)
- Safari ... After Taika(A.D. 645)

### Response to New Era

Support for new era names starting from 2019 is supported by the user's browser (*).

\(*) It depends on the browser from which the user accesses the customized kintone app, not the browser used to create customizations in Customine.

At the time of the first release of Customine (March 2018), no browsers are supported yet. When the browser is supported, the new era will be supported when the user updates the browser.
