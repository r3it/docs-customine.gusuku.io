---
title: Add Marker to Map
date: 2018-01-22T16:07:50+09:00
weight: 1520
---
## Summary

Adds a marker to an already installed map.

## How to use

[Display a map in a space](../show_google_map/) and [Show map in menu position](../show_google_map_at_menu) to set up a map.

For faster display, it is a good idea to have latitude and longitude information in the app. Longitude and latitude are displayed faster than if you specify an address.

When used in the list screen, it repeats the number of records in the list.

### Parameters to set

Set “Map”, “Address or Latitude/Longitude” and “Marker Name”.

#### Map

Choose which map you want the marker to appear on.

#### Address or latitude/longitude

Specify the location on the map.

When specifying an address, you can specify a detailed address up to the street number or a rough address such as a city name. In addition, in the case of famous buildings such as “Tokyo Sky Tree”, the name of the building can be displayed alone. These are the features of the GTS.

When specifying latitude and longitude, set the latitude and longitude numbers separated by commas.

```
34.687315, 135.526201
```

If the field contains address information, you can use an expression to pass the value of the field. If the field is divided into Region, Address1, and Address2:

```
${Region} ${Address1} ${Address2}
```

#### Marker Name

Sets the name of the marker. If omitted, the name of the marker will be the name of the marker if “Address or Latitude/Longitude” is specified in the address.

## Limitations

When used in the list screen, it repeats the number of records in the list.

At this time, if you specify an address instead of latitude and longitude in “Address or latitude/longitude”, you will wait about 2 seconds each time you place a marker. Therefore, it takes a long time to display all markers.

This is due to a limitation in Google Maps that the process of finding a location from an address cannot be called repeatedly in a short time.

To work around this limitation, specify latitude and longitude, not address.
