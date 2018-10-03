---
title: Show Map at Spacer
date: 2018-01-22T16:07:50+09:00
weight: 1500
---
## Summary

Display the map in the space.

## How to use

Place a space field to display the map. The element ID must be set in the space field.

You should also get an API key from the Google Maps site. To obtain an API key, see

https://developers.google.com/maps/documentation/javascript/get-api-key?hl=ja

for more information.

### Parameters to set

Set “Space”, “API Key”, “Address or Latitude/Longitude”, “Zoom Level”, and “Marker Name”.

#### Space

Specifies the space in which to display the map.

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

Cannot be used in the list screen.

Smartphone app is not supported.

### View more than two maps

If you repeat “Show Map in Space” with the same action number, it will be considered the same map, and only one map will be displayed.The second action does not change the currently displayed map position.

If you run “Show Map in Space” with different action numbers, each map will be displayed separately.

If you want to add more markers, instead of repeating “Show Map in Space”, you can use the [Add markers to a map](../add_google_map_marker) for more information.
