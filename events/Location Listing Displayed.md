# Location Listing Displayed

### This event is part of the page load sequence, including virtual page loads in the case of single page apps, and must be pushed between the `Page Load Started` and `Page Load Completed` events.

## Javascript Code
```js
window.appEventData000 = window.appEventData000 || [];
appEventData000.push({
  "event": "Location Listing Displayed",
    "listingDisplayed": {
        "filterList": "<filterList>",
        "listing": [
            {
                "isDisplayed": "<isDisplayed>",
                "itemPosition": "<itemPosition>",
                "location": {
                    "locationDistanceFromPOI": "<locationDistanceFromPOI>",
                    "locationId": "<locationId>"
                },
                "price": {
                    "currency": "<currency>"
                },
                "room": {
                    "numUnitsAvailable": "<numUnitsAvailable>"
                }
            }
        ]
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|currency|string|Currency of the prices given. ISO 4217 (3 character alpha), uppercase |USD, CAD, GBP, CHF|^[A-Z]{3}$|3|3||||
|filterList|string|A twice delimited string of filterType and filterValue pairs.  Use ~ between type and value.  Use | between pairs|sort~price ascending|color~green|size~medium|||||||
|isDisplayed|boolean|Helper node used by AA Product String Builder to set product scoped events|true|||||||
|itemPosition|integer|Integer position of a property within a sorted result. The first returned is position 1. For map results, this value can be the rank by distance from POI.|1, 2, 3, 4, 5||||0|||
|locationDistanceFromPOI|integer|The distance from the location to the user's point of interest|12, 3, 5, 200|||||||
|locationId|string|Unique Identifier of a Location. |155, 65588, 987764448|||||||
|numUnitsAvailable|integer|Integer number of rooms available for the given search parameters at a property or of a room type.|0, 10, 20, 23||||0|||
