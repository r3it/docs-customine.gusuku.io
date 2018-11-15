---
title: If Comparing Two Dates Satisfies Conditions
date: 2018-03-26T14:53:50+09:00
weight: 1110
---
## Summary

Compare two dates.

## How to use

This condition is used in conjunction with other “when” conditions.

For example, For example, you can set a condition that "end date" is within one month of "start date".

### Parameters to set

Specify “Date to compare (A)” “Condition”, “Date to compare (B)”, “Value to add or subtract from B”, and “Content to calculate (B)”.

In these five parameters, for example,

```
A >= B + a month
```

, and so on.

#### & Date to compare

Enter the date data you want to compare.

If you want to refer to the value of a date or time field

```
=Date_2
```

Refer to the field code with “=” as shown in.

To specify the current date, use the

```
=today()
```

in the Value field.

#### Condition

Select a comparison condition.

The subject is “A”; for example, if you choose “large”, the condition is “If A is greater than B”.

In this case, “greater” means “more future”.

#### Date to compare

Enter the date data you want to compare.

When you want to refer to a date or datetime field value, the input method is similar to A.

#### Value to add or subtract from B

If you want to add or decrease the number of days or months to B and then compare it to A.

For example, if you want to calculate “3 months from B”, select “○ months after” in “What to calculate (B)” and set “Value to add or subtract for B” to “3”.

If “Value to add or subtract from B” is set to “-3” and “What to calculate (B)” is set to “X months after”, “3 months from B” is calculated.

If you want to compare without calculating B as is, enter nothing.

If Calculate What is selected is Not Calculated, the number entered here is not used.

#### Calculated Content

If you want to add or decrease the number of days or months to B before comparing to A, select that unit of measure.

## About Handling of Time

If A or B is specified with a time, the date will be the date seen in the time zone of the logged-in user.

For example, if A is greater than B, then A is 2018-11-10 12:00, B 2018-11-10 11:00, A is greater than when looking at the time portion, but the time portion is ignored and considered the same day, so the greater than condition is not met.
