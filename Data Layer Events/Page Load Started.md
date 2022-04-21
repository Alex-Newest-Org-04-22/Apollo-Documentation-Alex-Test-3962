# Page Load Started

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ page_data: null });  // Clear the previous page_data object.
dataLayer.push({
  "event": "page_view",
  "detailed_event": "Page Load Started",
    "page_data": {
        "country": "<country>",
        "day_of_week": "<day_of_week>",
        "email_recipient_id": "<email_recipient_id>",
        "hour": "<hour>",
        "language": "<language>",
        "nameAlex": "<nameAlex>",
        "owner": "<owner>",
        "page_location": "<page_location>",
        "page_name_detailed": "<page_name_detailed>",
        "page_titleAlex": "<page_titleAlex>",
        "typeAlex": "<typeAlex>",
        "weekday_or_weekend": "<weekday_or_weekend>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|page_data.country|string|The country the site is associated with.||||||||
|page_data.day_of_week|string|The day of the week the activity occured.||||||||
|page_data.email_recipient_id|string|Captures the ID of the recipient to whom an email was sent||||||||
|page_data.hour|string|The time of activity at the top of the hour.||||||||
|page_data.language|string|The language of the current page, usually pulled from the &lt;html&gt; tag lang attribute.||||||||
|page_data.nameAlex|string|Captures the name of the page the user is on|product - XYZ123, Mens - Tops - Sweaters, Order Confirmation|||||||
|page_data.owner|string|Captures the licensee or owner of content \(i.e. HBO\).|XX product management, marketing, vendor name|||||||
|page_data.page_location|string|The url of the page currently being viewed.||||||||
|page_data.page_name_detailed|string|Captures the full detail of the page the user is on \(usage is flexible\)|product - XYZ123 - super cotton neck scarf, Mens - Tops - Sweaters - Supmina, Wool, Rayon, Order Confirmation - 098fghjkl|||||||
|page_data.page_titleAlex|string|The title of the page currently being viewed, generally available in &lt;title&gt;.||||||||
|page_data.typeAlex|string|The type of page currently viewed.|home, pdp, article|||||||
|page_data.weekday_or_weekend|string|Whether it was a weekday or weekend when the activity occurred.||||||||




