# Product Added to Registry

### 

## Javascript Code
```js
window.appEventData000 = window.appEventData000 || [];
appEventData000.push({
  "event": "Product Added to Registry",
    "product": [
        {
            "productInfo": {
                "productID": "<productID>"
            }
        }
    ],
    "registry": {
        "registryID": "<registryID>",
        "registryType": "<registryType>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|productID|string|Unique Identifier of a product or offering.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level above SKU for products with SKU variants. |155, 65588, 987764448|||||||
|registryID|string|Back-end identifier for a gift registry |12345, 435678, 34567, XCV456, XCV876|||||||
|registryType|string|The type of gift registry|Wedding, Baby, Birth Day, Anniversary|||||||
