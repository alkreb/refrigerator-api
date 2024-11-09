---
layout: page
---

# `freezer` resource

Base endpoint:

```shell

{server_url}/freezer
```

Contains information about freezer items for the users of the service.

## Resource properties

Sample `freezer item` resource

```js

{
    "category": "meal prep",
    "type": "dinner",
    "subtype": "burritos",
    "description": "5 burritos prepared ahead",
    "date_frozen": "12/28/2024",
    "purchased_date": "NA",
    "use_by_date": "02/28/2025",
    "freezer_section": "bottom shelf",
    "id": 1
}
```

| Property name     | Type   | Description                                     |
| ----------------- | ------ | ----------------------------------------------- |
| `category`        | string | The category of the item                        |
| `type`            | string | The type of the item                            |
| `subtype`         | string | The subtype of the item                         |
| `description`     | string | The item description                            |
| `date_frozen`     | string | The date the item was frozen                    |
| `purchased_date`  | string | The purchase date of the item                   |
| `use_by_date`     | string | The use-by date of the item                     |
| `freezer_section` | string | The storage location of the item in the fridge  |
| `id`              | number | The ID of the item                              |

## READ

* [Get all items _(coming soon)_](#resource-properties)
* [Get item by ID _(coming soon)_](#resource-properties)