---
nav_order: 2
---

# `fridge` resource

Base endpoint:

```shell

{server_url}/fridge
```

Contains information about fridge items for the users of the service.

## Resource properties

Sample `fridge item` resource

```js

{
    "category": "dairy",
    "type": "cheese",
    "subtype": "deli sliced pepper jack",
    "description": "",
    "sell_by_date": "NA",
    "best_by_date": "12/28/2024",
    "purchase_date": "07/01/2024",
    "fridge_section": "middle shelf",
    "id": 1
}
```

| Property name    | Type   | Description                                     |
| ---------------- | ------ | ----------------------------------------------- |
| `category`       | string | The category of the item                        |
| `type`           | string | The type of the item                            |
| `subtype`        | string | The subtype of the item                         |
| `sell_by_date`   | string | The sell-by date of the item                    |
| `best_by_date`   | string | The best-by date of the item                    |
| `purchase_date`  | string | The purchase date of the item                   |
| `fridge_section` | string | The storage location of the item in the fridge  |
| `id`             | number | The ID of the item                              |

## READ

* [Get all items _(coming soon)_](#resource-properties)
* [Get item by ID _(coming soon)_](#resource-properties)
