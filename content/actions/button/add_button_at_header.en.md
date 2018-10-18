---
title: Place Button in Header
date: 2018-01-22T16:07:50+09:00
weight: 1210
---
## Summary

Places the button at the specified location (menu position).

By combining with the condition of [When the button is pressed](../../../conditions/condition_other/button_clicked), you can customize to perform some action when you press a button.

## How to use

When you place a button, it only appears on the screen, and when you press it, nothing happens. To customize something to do when you press a button, place another action and add the [When the button is pressed](../../../conditions/condition_other/button_clicked) condition.

You can also place more than one button in a single location.In this case, buttons are added from left to right in the order in which the actions are performed.

### Parameters to set

Set Location Label.

#### Location

Choose where to place the button.

-	Above Record Details menu... It is displayed in the position of the following figure on the record detail screen or the edit screen.

![Above Record Details menu](/images/ja/actions/button/add_button_at_header/1.png)

-	To the right of the list menu... It is displayed in the position shown below in the record list screen.

![To the right of the list menu](/images/ja/actions/button/add_button_at_header/2.png)

-	Below the list screen menu... It is displayed in the position shown below in the record list screen.

![Below the list screen menu](/images/ja/actions/button/add_button_at_header/3.png)

#### Label

Specifies the label that appears on the button when it is displayed on the screen.

## Advanced Information

The button will have the following CSS class name:

-	customine-button
-	At the top of the record details screen: customine-at-record-header-menu-space
-	On the right side of the list screen: customine-at-header-menu-space
-	In the lower part of the list screen menu: customine-at-header-space

You can also use ID.

-	customine-button-action-## (for example, customine-button-1)


This allows you to customize the style of buttons by registering a css file in your app.

## Limitations

“Top of the record details screen” cannot be used in the list screen.

“Right side of list screen menu” and “Bottom side of list screen menu” cannot be used outside of list screen.

“Right side of list screen menu” is not supported in the mobile version app.
