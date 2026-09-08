# Schemas: budgetCategory

Property tables for definitions owned by `budgetCategory`.

Record page: [budgetCategory](../records/budgetCategory.md).

## Index

- [budgetCategory](#budgetcategory) — 7 properties
- [budgetCategoryCollection](#budgetcategorycollection) — 6 properties

## budgetCategory

Browser definition `budgetCategory`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `budgetType` | Global | boolean |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## budgetCategoryCollection

Browser definition `budgetCategoryCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | budgetCategory[] |  |  | [`budgetCategory`](#budgetcategory) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |
