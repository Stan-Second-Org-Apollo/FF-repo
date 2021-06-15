# Accommodation Booking Started

### 

## Javascript Code
```js
window.appEventData000 = window.appEventData000 || [];
appEventData000.push({
  "event": "Accommodation Booking Started",
    "booking": {
        "roomList": [
            {
                "room": {
                    "numberInMultiRoomReservation": "<numberInMultiRoomReservation>",
                    "rateCode": "<rateCode>",
                    "ratePerNight": "<ratePerNight>",
                    "stayDate": "<stayDate>",
                    "typeCode": "<typeCode>"
                }
            }
        ]
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|numberInMultiRoomReservation|integer|Integer position of a room in a multi-room booking action.|1, 2, 3||||1|||
|rateCode|string|Description of the rate being offered. Should match rate codes from back-end systems to allow data import. |AAA, MILITARY, CORP-567, CORP-345|||||||
|ratePerNight|string|String representation of the price per use-period. Typically nightly rate for a hotel room or monthly rate for an apartment. Positive. Up to two decimal places for cents. No currency symbol.|200, 75.29, 150, 89.2|^[0-9]*(\.[0-9]{1,2})?$||||||
|stayDate|string|Date of each room night. ISO 8601 form (YYYY-MM-DD). Jan 1, 2019 is 2019-01-01|2001-12-22, 2011-01-01|^([0-9]{4})-(1[0-2]|0[1-9])-(3[01]|0[1-9]|[12][0-9])$||||||
|typeCode|string|A code describing the room features. Often indicates number of beds, smoking or non-smoking, ADA accessibility and so on.|1-K-NS, 2-Q-S, S-K-NS-City|||||||
