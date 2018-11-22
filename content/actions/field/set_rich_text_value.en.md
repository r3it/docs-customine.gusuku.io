---
title: Set Rich Text Text Field Value
date: 2018-01-22T16:07:50+09:00
weight: 1404
---
## Overview

Sets the value of the rich editor field field, which can include line breaks and styles.

## How to use

### Parameters to set

Set FieldValue.

#### field

Select the field you want to set to.

#### value

Sets the value to set.

If you want to put the value of another field in a string, use the expression ${field}.

## Please note

If you want to apply a style to the ${field} part, such as font color or font size, select the entire ${field} from “${” to “}” and apply the style. If you apply a style to only the “field” part, except for the ${} part, the field value will not be correct.

## Known Issues

If the text size and text color are changed at the same time, the text color setting is not reflected in the kintone app, but only the text size is reflected.
