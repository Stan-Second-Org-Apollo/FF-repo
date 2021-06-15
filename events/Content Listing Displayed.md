# Content Listing Displayed

### This event is part of the page load sequence, including virtual page loads in the case of single page apps, and must be pushed between the `Page Load Started` and `Page Load Completed` events.

## Javascript Code
```js
window.appEventData000 = window.appEventData000 || [];
appEventData000.push({
  "event": "Content Listing Displayed",
    "listingDisplayed": {
        "listing": [
            {
                "content": {
                    "contentDate": "<contentDate>"
                },
                "isDisplayed": "<isDisplayed>"
            }
        ]
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|contentDate|string|Date of the content's publication. ISO 8601 form (YYYY-MM-DD). Jan 1, 2019 is 2019-01-01|2001-12-22, 2011-01-01|^([0-9]{4})-(1[0-2]|0[1-9])-(3[01]|0[1-9]|[12][0-9])$||||||
|isDisplayed|boolean|Helper node used by AA Product String Builder to set product scoped events|true|||||||
