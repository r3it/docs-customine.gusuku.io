---
title: Show Map in Header
date: 2018-01-22T16:07:50+09:00
weight: 1510
---
## Summary

Places the map at the specified location (menu position).

## How to use

Before you go to the Google Maps site, get an API key. To obtain an API key, see

https://developers.google.com/maps/documentation/javascript/get-api-key

for more information.

### Parameters to set

Set “Location”, “API Key”, “Address or Latitude/Longitude”, “Zoom Level”, and “Marker Name”.

#### Location

Specifies where you want the map to appear.

-	Above Record Details menu... It is displayed in the position of the following figure on the record detail screen or the edit screen.

![Above Record Details menu](/images/ja/actions/external/show_google_map_at_menu/1.png)

-	To the right of the list menu... It is displayed in the position shown below in the record list screen.

![To the right of the list menu](/images/ja/actions/external/show_google_map_at_menu/2.png)

-	Below the list screen menu... It is displayed in the position shown below in the record list screen.

![Below the list screen menu](/images/ja/actions/external/show_google_map_at_menu/3.png)

#### API Key

Enter the Google Maps API key.

Get the API key from the Google Maps site.

https://cloud.google.com/maps-platform/?hl=jahttps://developers.google.com/maps/documentation/javascript/get-api-key?hl=ja

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

#### Zoom Level

Enter the zoom level.

Depending on the Google Maps documentation, consider the following:

-	1: World
-	5: Continent
-	10: City
-	15: Street
-	20: Building

https://developers.google.com/maps/documentation/javascript/tutorial?hl=ja#MapOptions

#### Marker Name

Sets the name of the marker. If omitted, the name of the marker will be the name of the marker if “Address or Latitude/Longitude” is specified in the address.

## Limitations

“Top of the record details screen” cannot be used in the list screen.

“Right side of list screen menu” and “Bottom side of list screen menu” cannot be used outside of list screen.

Only the bottom of the list screen menu is supported in the smartphone version app.

### View more than two maps

If you repeat “Show Map at Menu Position” with the same action number, it will be considered the same map and only one map will be displayed.The second action does not change the currently displayed map position.

If you run “Show Map at Menu Position” with different action numbers, each map will be displayed separately.

If you want to increase markers, do not repeat “Show map at menu position”. [Add markers to a map](../add_google_map_marker) for more information.
