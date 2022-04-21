# Order Placed

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ ecommerce: null });  // Clear the previous ecommerce object.
dataLayer.push({
  "event": "purchase",
  "detailed_event": "Order Placed",
    "ecommerce": {
        "currency": "<currency>",
        "items": [
            {
                "item_business_unit": "<item_business_unit>",
                "item_id": "<item_id>",
                "item_is_web_exclusive": <item_is_web_exclusive>,
                "item_name": "<item_name>",
                "sku": "<sku>",
                "third_party_vendor_id": "<third_party_vendor_id>"
            }
        ],
        "transaction_id": "<transaction_id>",
        "value": <value>
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|ecommerce.currency|string|The currency, in 3-letter ISO 4217 format.||||||||
|ecommerce.items[n].item_business_unit|string|Captures the business unit associated with each product.|Apparel, Shoes, Home|||||||
|ecommerce.items[n].item_id|string|Item ID \(context-specific\).The product primary ID \(SKU or UPC\)|SKU\_12345|||||||
|ecommerce.items[n].item_is_web_exclusive|boolean|Captures if the product is exclusively sold on the website||||||||
|ecommerce.items[n].item_name|string|Item Name \(context-specific\).|jeggings|||||||
|ecommerce.items[n].sku|string||34567890, 4567890, 00155-large-cornflower|||||||
|ecommerce.items[n].third_party_vendor_id|string|Captures the vendor id of the third party vendor associated with product conversion.||||||||
|ecommerce.transaction_id|string|The unique identifier of a transaction.|T\_12345, 19283j2nm9jdjs|^[a-zA-Z0-9]{6,20}$|6|20||||
|ecommerce.value|number|The monetary value of the event.|7.77, 239.55, 659|||||||




