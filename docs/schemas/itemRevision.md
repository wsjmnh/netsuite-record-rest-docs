# Schemas: itemRevision

Property tables for definitions owned by `itemRevision`.

Record page: [itemRevision](../records/itemRevision.md).

## Index

- [itemRevision](#itemrevision) — 10 properties
- [itemRevisionCollection](#itemrevisioncollection) — 6 properties
- [itemRevisionSelectOptions](#itemrevisionselectoptions) — 1 properties

## itemRevision

Browser definition `itemRevision`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `effectiveDate` | Effective Date | string | date |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `inactive` | Inactive | boolean |  |  |  |  |
| `item` |  | assemblyItem |  |  | [`assemblyItem`](assemblyItem.md#assemblyitem) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `memo` | Memo | string |  |  |  |  |
| `name` | Name | string |  |  |  |  |
| `obsoleteDate` | Obsolete Date | string | date |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## itemRevisionCollection

Browser definition `itemRevisionCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | itemRevision[] |  |  | [`itemRevision`](#itemrevision) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## itemRevisionSelectOptions

Browser definition `itemRevisionSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `item` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
