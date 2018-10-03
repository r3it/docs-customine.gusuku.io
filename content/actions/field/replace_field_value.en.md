---
title: フィールドの値の一部を文字列置換する
date: 2018-01-22T16:07:50+09:00
weight: 1520
---
## Summary

Replaces part of a string in a field with another string.

## How to use

### Parameters to set

Specify here “Field”, “Replace with string” and “If multiple hits”.

For example, if you specify “Grams” for “Replace With” and “g” for “Replace With”, 3.5 grams will be replaced by “3.5g”.

#### field

Select the field you want to replace. Multiple selections are allowed, and all selected fields are replaced at the same time.

The available field types are:

-	String (one line)
-	String (multiple lines)
-	Rich Editor
-	Link

#### Replace with

Enter the string you want to replace.

#### Replace with

Enter the replacement string. If this parameter is empty, it means that the replace will remove the “replace string”.

#### If you hit more than one hit

Select the behavior when there are multiple occurrences in the “From” field value: “Replace All” or “Replace First One”.

Select “Replace All” to replace all occurrences of “Replace With”. If you select “Replace the first one”, only the first one found (the previous one as a sentence) will be replaced.

## Limitations

You cannot use a regular expression for Replace With.
