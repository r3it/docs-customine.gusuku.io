---
title: Search Address from Zip Code (Japanese Only)
date: 2018-01-22T16:07:50+09:00
weight: 1541
---
## Summary

**For use in Japan only.**

Provides the ability to search for an address by entering a postal code and automatically fill in the form.

## How to use

For example, if you want to perform a search when you press a button like “Search Address”, place the button beforehand.

### Parameters to set

Set the Postal Code Field, State Field, Address (1) Field, Address (4) Field.

#### Postal Code Field

Specifies the field in which you want to enter a postal code value.

#### State Field

Specifies the field to which you want to set the name of the state returned in the search results.

If the destination is a select field, such as a drop-down, the choice must end with “prefecture”, for example, “Toyama Prefecture”.If you omit “prefecture”, such as “Toyama”, you will get an error.

#### Address (1) field

#### Address (2) field

#### Address (3) field

#### Address (4) field

Select the field in which you want to set addresses after the city name.

Typically, address (1) is the city name, address (2) is the town name, and address (3) (4) is the reserve.

Address (1) through Address (4) can be in the same field.In this case, you can combine the name of the city, the name of the city, and the name of the city, and set it to a single field.

### Limitations

The following field types can be selected under Postal Code Fields:

-	String (one line)
-	Drop-down

The following field types can be selected in “State field”:

-	String (one line)
-	String (multiple lines)
-	Rich Editor
-	Drop-down

The following field types can be selected from “Address (1) Field” to “Address (4) Field”:

-	String (one line)
-	String (multiple lines)
-	Rich Editor
