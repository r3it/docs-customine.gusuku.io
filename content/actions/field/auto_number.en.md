---
title: Auto Number
date: 2018-01-22T16:07:50+09:00
weight: 1560
---
## Summary

Automatically number the field and set it to the field.

## How to use

When the action is executed, it communicates with the numbering server and sets the retrieved value to the specified field.

Communication occurs, so depending on the communication environment, it may take some time for the value to be set.

### Parameters to set

Set the “field” and the parameters that determine the numbering rules.

#### field

Select the field to which you want to set the numbered values.

The value of the field is set in a fematted state, such as zero padded.

You can omit this parameter if you do not want to immediately set the value in the field, and you want to use the numbered value for another action.

#### App Unit Numbering

If you select None, the numbering will be sequential across the entire domain.

If you select “Number by app”, the sequence number is managed for each app.

#### Zero padding

With zero padding, if less than the number of digits specified in the next number of digits is zero padded.

For zero padding, the number of digits must be greater than or equal to 1.

For example, if zero padding is “8” and the number of digits is “1”, the field will be set to “00000001”.

#### Digits

Specifies the number of decimal spaces for zero padding. Otherwise, this parameter is ignored.

If the number is greater than this number of digits, the number of digits cut is **Not done**. For example, if the number “1234” is taken with the number “3”, the value “1234” will be set instead of being cut to “123” or “234”.

#### Prefix string

Specify if you want a fixed string to precede the picked number.

#### String to append (suffix)

Specify if you want to append a fixed string after the number.

#### Numbering Cycle

If you choose None, the number will not be reset.

If you select “Numbering by Month”, the sequence number will be reset to 1 in the following month.

Select “Numbering by Year” to reset the sequence number to 1 on January 1st of the year. Note that this is a year, not a year.

#### Time Zone

If you select monthly or yearly units for the numbering cycle, select which country or region you want to base the time on.

### Limitations

The following field types can be selected under Field:

-	String (one line)
-	Number

If you select a number with a prefix or suffix, you will get an error when you perform the action.
