# Location Listing Item Clicked

### This event is part of the page load sequence, including virtual page loads in the case of single page apps, and must be pushed between the `Page Load Started` and `Page Load Completed` events.

## Javascript Code
```js
window.appEventData000 = window.appEventData000 || [];
appEventData000.push({
  "event": "Location Listing Item Clicked",
    "listingDisplayed": {
        "sortOrder": "<sortOrder>"
    },
    "listingItemClicked": {
        "listing": [
            {
                "price": {
                    "currency": "<currency>"
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
|sortOrder|string|Indicates the sort order.|high-low, low-high, nearest-farthest, a-z, newest-oldest|||||||
