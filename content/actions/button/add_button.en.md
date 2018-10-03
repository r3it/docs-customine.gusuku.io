---
title: Place Button at Spacer
date: 2018-01-22T16:07:50+09:00
weight: 1200
---
## Summary

Places the button at the specified location (space).

By combining with the condition of [When the button is pressed](../../../conditions/condition_other/button_clicked), you can customize to perform some action when you press a button.

## How to use

When you place a button, it only appears on the screen, and when you press it, nothing happens. To customize something to do when you press a button, place another action and add the [When the button is pressed](../../../conditions/condition_other/button_clicked) condition.

You can also have multiple buttons in a single space field.In this case, buttons are added from left to right in the order in which the actions are performed.

### Get ready

Make sure you have a space field in which you want to place buttons in your app. The element ID must be set in the space field.

### Parameters to set

Set Location Label.

#### Location

Specifies the space field on which to place the button.

#### Label

Specifies the label that appears on the button when it is displayed on the screen.

## Advanced Information

The button will have the following css class name:

-	customine-button
-	customine-at-spacer

You can also use the

-	customine-button-action number (for example, customine-button-1)

will be attached.

This allows you to customize the style of buttons by registering a css file in your app.

## Limitations

Cannot be used in the list screen.

Smartphone app is not supported.
