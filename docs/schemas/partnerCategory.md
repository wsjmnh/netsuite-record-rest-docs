# Schemas: partnerCategory

Property tables for definitions owned by `partnerCategory`.

Record page: [partnerCategory](../records/partnerCategory.md).

## Index

- [partnerCategory](#partnercategory) — 7 properties
- [partnerCategoryCollection](#partnercategorycollection) — 6 properties
- [partnerCategorySelectOptions](#partnercategoryselectoptions) — 1 properties

## partnerCategory

Browser definition `partnerCategory`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Partner Category/Role | string |  |  |  |  |
| `parent` |  | partnerCategory |  |  | [`partnerCategory`](#partnercategory) |  |
| `refName` | Reference Name | string |  |  |  |  |

## partnerCategoryCollection

Browser definition `partnerCategoryCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | partnerCategory[] |  |  | [`partnerCategory`](#partnercategory) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## partnerCategorySelectOptions

Browser definition `partnerCategorySelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `parent` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
