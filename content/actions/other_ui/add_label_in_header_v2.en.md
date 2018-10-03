---
title: Diaplay Text in Header
date: 2018-01-22T16:07:50+09:00
weight: 1545
---
## Summary

Displays characters (text) at the specified location (menu position).

[“Change the Text Displayed at the Space Menu Position”](../set_label_text_v2), you can use theYou can change the text displayed on the screen depending on your situation.

## How to use

### Parameters to set

Set Location Text to Display.

#### Location

Select a location to display.

-	Above Record Details menu... It is displayed in the position of the following figure on the record detail screen or the edit screen.

![Above Record Details menu](/images/ja/actions/button/add_button_at_header/1.png)

-	To the right of the list menu... It is displayed in the position shown below in the record list screen.

![To the right of the list menu](/images/ja/actions/button/add_button_at_header/2.png)

-	Below the list screen menu... It is displayed in the position shown below in the record list screen.

![Below the list screen menu](/images/ja/actions/button/add_button_at_header/3.png)

#### Text to display

Specifies the text to display on the screen.

You can decorate characters or embed expressions inside text.

## Advanced Information

The text will have the following CSS class name:

-	customine-label
-	At the top of the record details screen: customine-at-record-header-menu-space
-	On the right side of the list screen: customine-at-header-menu-space
-	In the lower part of the list screen menu: customine-at-header-space

You can also use ID.

-	customine-label-action-## (for example, customine-label-1)

This allows you to customize the style of buttons by registering a css file in your app.

## Limitations

“Top of the record details screen” cannot be used in the list screen.

“Right side of list screen menu” and “Bottom side of list screen menu” cannot be used outside of list screen.

Only the bottom of the list screen menu is supported in the smartphone version app.
