---
title: Add Label in Header
date: 2018-01-22T16:07:50+09:00
weight: 1546
---
## Summary

Places the label at the specified location (menu position).

[Set text to added labels (old)](../set_label_text), you can use theYou can change the text displayed on the screen depending on your situation.

## Deprecated

This will be an older version, so you can use the [New Version](../add_label_in_header_v2/) for more information.

## How to use

### Parameters to set

Set Name, Location, and Text to Display.

#### Name

Type a name that identifies the name of the item. This name does not appear on the kintone screen. [Set Text to Added Label](../set_label_text)to specify which label to set.

#### Location

Select where you want to place the label.

-	Above Record Details menu... It is displayed in the position of the following figure on the record detail screen or the edit screen.

![Above Record Details menu](/images/ja/actions/button/add_button_at_header/1.png)

-	To the right of the list menu... It is displayed in the position shown below in the record list screen.

![To the right of the list menu](/images/ja/actions/button/add_button_at_header/2.png)

-	Below the list screen menu... It is displayed in the position shown below in the record list screen.

![Below the list screen menu](/images/ja/actions/button/add_button_at_header/3.png)

#### Text to display

Specifies the text to display on the screen.

It is possible to decorate characters using HTML tags.

## Limitations

“Top of the record details screen” cannot be used in the list screen.

“Right side of list screen menu” and “Bottom side of list screen menu” cannot be used outside of list screen.

Only the bottom of the list screen menu is supported in the smartphone version app.
