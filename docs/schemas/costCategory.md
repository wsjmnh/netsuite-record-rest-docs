# Schemas: costCategory

Property tables for definitions owned by `costCategory`.

Record page: [costCategory](../records/costCategory.md).

## Index

- [costCategory](#costcategory) — 13 properties
- [costCategoryCollection](#costcategorycollection) — 6 properties
- [costCategorySelectOptions](#costcategoryselectoptions) — 2 properties

## costCategory

Browser definition `costCategory`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | account |  |  | [`account`](account.md#account) |  |
| `accountRequired` | Account Required | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `itemCostType` |  | object |  |  |  |  |
| `itemCostType.id` | Internal identifier | string |  |  |  | `MACHINERUN`, `LANDED`, `MATERIALOVERHEAD`, `MACHINESETUPOVERHEAD`, `LABORSETUP`, `OUTSOURCINGCHARGE`, `LABORSETUPOVERHEAD`, `MACHINESETUP`, `LABORRUNOVERHEAD`, `LABORRUN`, `SERVICE`, `MATERIAL`, `MACHINERUNOVERHEAD` |
| `itemCostType.refName` | Reference Name | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `longitemtype` |  | string |  |  |  |  |
| `name` | Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `tname` |  | string |  |  |  |  |

## costCategoryCollection

Browser definition `costCategoryCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | costCategory[] |  |  | [`costCategory`](#costcategory) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## costCategorySelectOptions

Browser definition `costCategorySelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `itemCostType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
