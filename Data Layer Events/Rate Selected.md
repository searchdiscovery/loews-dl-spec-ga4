# Rate Selected

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ ecommerce: null });  // Clear the previous ecommerce object.
dataLayer.push({
  "event": "add_to_cart",
  "detailed_event": "Rate Selected",
    "ecommerce": {
        "items": [
            {
                "arrival_date": "<arrival_date>",
                "days_before_start_date": <days_before_start_date>,
                "departure_date": "<departure_date>",
                "item_id": "<item_id>",
                "item_name": "<item_name>",
                "market_code": "<market_code>",
                "number_of_adults": <number_of_adults>,
                "number_of_children": <number_of_children>,
                "quantity": <quantity>,
                "room_rate_code": "<room_rate_code>",
                "room_type_code": "<room_type_code>"
            }
        ]
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|ecommerce.items[n].arrival_date|string|the arrival date of a booking|YYYY-MM-DD|||||||
|ecommerce.items[n].days_before_start_date|number|captures the Days Before Start Date of the booking||||||||
|ecommerce.items[n].departure_date|string|captures Departure Date of the booking||||||||
|ecommerce.items[n].item_id|string|Please reference this document to determine the Item ID
https:\/\/docs.google.com\/spreadsheets\/d\/1PDhNOzXI9E7jZ9obejV4owtW3Wtwq66\_IaN-CBoHbRs\/edit\#gid=1543857253|6558, 70561|||||||
|ecommerce.items[n].item_name|string|Item Name \(context-specific\).|jeggings|||||||
|ecommerce.items[n].market_code|string|captures the Market Code of the booking||||||||
|ecommerce.items[n].number_of_adults|integer|Captures the number of adults in a booking||||||||
|ecommerce.items[n].number_of_children|integer|captures the Number of Children in a booking \(ecommerce DE\)||||||||
|ecommerce.items[n].quantity|integer|Captures the number of nights in the booking||||||||
|ecommerce.items[n].room_rate_code|string|captures the rate code of the room||||||||
|ecommerce.items[n].room_type_code|string|captures the room type code of the booking||||||||

## Attached Notes

<p>User selects a rate.</p>
<p>On reservations.loewshotels.com, this is the "Select This Rate" button</p>
<p>on be.synxis.com, this is the <span style="font-weight: 400;">&ldquo;Book Now&rdquo; button.</span></p>
