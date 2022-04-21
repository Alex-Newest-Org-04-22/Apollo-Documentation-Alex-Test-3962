# Product Viewed

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ ecommerce: null });  // Clear the previous ecommerce object.
dataLayer.push({
  "event": "view_item",
  "detailed_event": "Product Viewed",
    "ecommerce": {
        "competitor_pricing": "<competitor_pricing>",
        "currency": "<currency>",
        "items": [
            {
                "item_id": "<item_id>",
                "item_name": "<item_name>",
                "item_out_of_stock": <item_out_of_stock>,
                "sku": "<sku>"
            }
        ],
        "value": <value>
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|ecommerce.competitor_pricing|string|Captures the product ID, current price and competitor price for each product.||||||||
|ecommerce.currency|string|The currency, in 3-letter ISO 4217 format.||||||||
|ecommerce.items[n].item_id|string|Item ID \(context-specific\).The product primary ID \(SKU or UPC\)|SKU\_12345|||||||
|ecommerce.items[n].item_name|string|Item Name \(context-specific\).|jeggings|||||||
|ecommerce.items[n].item_out_of_stock|boolean|Count of times that products were out of stock on initial view of product detail page.|TRUE, FALSE|||||||
|ecommerce.items[n].sku|string||34567890, 4567890, 00155-large-cornflower|||||||
|ecommerce.value|number|The monetary value of the event.|7.77, 239.55, 659|||||||




