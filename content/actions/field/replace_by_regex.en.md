---
title: Replace by Regular Expression
date: 2018-01-22T16:07:50+09:00
weight: 1525
---
## Summary

Replaces the part of a field that matches the regular expression with another string.

## How to use

### Parameters to set

Set “Field”, “Regular Expression”, “Replace String” and “Multiple hits”.

#### field

Select the field you want to replace. Multiple selections are allowed, and all selected fields are replaced at the same time.

The available field types are:

-	String (one line)
-	String (multiple lines)
-	Rich Editor
-	Link

#### Regular expression

Enter a regular expression.

Example

```
(\d+)-(\d+)-(\d+)
```

#### Substitution Strings

Enter a string to replace the hit.If this parameter is empty, it means that the replace will remove the “replace string”.

For... to replace a submatch string that is caught in parentheses () in the regular expression.In this case, however, be careful not to be confused with $1 in the Customine formula functionality, that is, referencing the results of other actions.

Example: Replace with parentheses in a regular expression. (It is not an expression, so do not begin with “=”.)

```
$1/$2/$3/
```

For example: Replace with the results of another action. (If you use a Customine expression, start with “=”.)

```
=$1
```

#### If you hit more than one hit

Select the behavior when there are multiple occurrences in the “From” field value: “Replace All” or “Replace First One”.

Select “Replace All” to replace all occurrences of “Replace With”.If you select “Replace the first one”, only the first one found (the previous one as a sentence) will be replaced.

## Limitations

Regular expression matching and replacement operations use the JavaScript standard RegExp.Therefore, the fine-grained behavior of regular expressions, such as available special characters, depends on the RegExp implementation of the web browser.
