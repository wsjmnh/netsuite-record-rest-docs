# Schemas: otherNameCategory

Property tables for definitions owned by `otherNameCategory`.

Record page: [otherNameCategory](../records/otherNameCategory.md).

## Index

- [otherNameCategory](#othernamecategory) — 6 properties
- [otherNameCategoryCollection](#othernamecategorycollection) — 6 properties

## otherNameCategory

Browser definition `otherNameCategory`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Type | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## otherNameCategoryCollection

Browser definition `otherNameCategoryCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | otherNameCategory[] |  |  | [`otherNameCategory`](#othernamecategory) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |
