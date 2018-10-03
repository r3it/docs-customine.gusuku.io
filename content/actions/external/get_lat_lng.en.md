---
title: Acquire Latitude and Longitude from Address
date: 2018-01-22T16:07:50+09:00
weight: 1530
---
## Summary

Use the Google Maps API to get the latitude and longitude from an address and set it to a field.

## How to use

Before you go to the Google Maps site, get an API key. To obtain an API key, see

https://developers.google.com/maps/documentation/javascript/get-api-key?hl=ja

for more information.

Set up a field in your app to store latitude and longitude. Latitude and longitude can be a separate field or the same field.

### Parameters to set

Set “API Key”, “Address”, “Latitude Field” and “Longitude Field”.

#### API Key

Enter the Google Maps API key.

Get the API key from the Google Maps site.

https://cloud.google.com/maps-platform/?hl=jahttps://developers.google.com/maps/documentation/javascript/get-api-key?hl=ja

#### Address

Enter the address for which you want to retrieve latitude and longitude.

If the field contains address information, you can use an expression to pass the value of the field. If the field is divided into Region, Address1, and Address2:

```
${Region} ${Address1} ${Address2}
```

You can specify a detailed address to the street address, or a rough address such as a city name. In addition, in the case of famous buildings such as “Tokyo Sky Tree”, the name of the building can be obtained by itself. These are the features of the GTS.

#### Latitude field

Select the field in which you want to store the retrieved latitude data.

You can select a string (single line) or a numeric field.

If you want to store latitude and longitude in the same field, select a string (one line) type field instead of a numeric field.

#### Longitude field

Select the field in which you want to store the retrieved longitude data.

You can select a string (single line) or a numeric field.

If you want to store latitude and longitude in the same field, select a string (one line) type field instead of a numeric field.

If you store latitude and longitude in the same field,

```
34.6937,135.5022
```

The latitude and longitude are set, separated by commas, as shown in.

## Limitations

When you specify a field (column) in the table in the latitude and longitude fields, theGets the latitude and longitude for each row in the table.

Because of the limitations of the Google Maps API, you cannot get a lot at once.Acquisition is carried out at intervals of approximately 2 seconds.

This will take a long time for all retrievals to complete. In the meantime, the user edits on the record editing screen are lost. Returns to the contents of the latitude and longitude retrieval process.

When you will get the latitude and longitude for a field in a table, we recommend to use [Show loading screen](../../other_ui/show_spinner/), and you should not allow user input.
