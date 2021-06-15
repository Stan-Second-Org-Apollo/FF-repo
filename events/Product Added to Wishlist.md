# Product Added to Wishlist

### 

## Javascript Code
```js
window.appEventData000 = window.appEventData000 || [];
appEventData000.push({
  "event": "Product Added to Wishlist",
    "eventDetails": {
        "multiAdditionDetail": "<multiAdditionDetail>",
        "multiAdditions": "<multiAdditions>"
    },
    "product": [
        {
            "productInfo": {
                "productID": "<productID>"
            }
        }
    ],
    "wishlist": {
        "wishlistID": "<wishlistID>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|multiAdditionDetail|string|Provides details of multiple product additions to carts, wishlists, registries, etc.|all items, 3 of 5, 2 of 4|||||||
|multiAdditions|boolean|Flag indicating whether multilple products where added to carts, wishlists, registries, etc.|true, false|||||||
|productID|string|Unique Identifier of a product or offering.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level above SKU for products with SKU variants. |155, 65588, 987764448|||||||
|wishlistID|string|Back-end identifier for a wishlist|12345, 435678, 34567, XCV456, XCV876|||||||
