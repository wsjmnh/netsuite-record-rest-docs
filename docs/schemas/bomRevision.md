# Schemas: bomRevision

Property tables for definitions owned by `bomRevision`.

Record page: [bomRevision](../records/bomRevision.md).

## Index

- [bomRevision](#bomrevision) — 14 properties
- [bomRevision-componentCollection](#bomrevision-componentcollection) — 6 properties
- [bomRevision-componentElement](#bomrevision-componentelement) — 15 properties
- [bomRevisionCollection](#bomrevisioncollection) — 6 properties
- [bomRevisionSelectOptions](#bomrevisionselectoptions) — 2 properties

## bomRevision

Browser definition `bomRevision`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `billOfMaterials` |  | bom |  |  | [`bom`](bom.md#bom) |  |
| `component` |  | bomRevision-componentCollection |  |  | [`bomRevision-componentCollection`](#bomrevision-componentcollection) |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `effectiveEndDate` | Effective End Date | string | date |  |  |  |
| `effectiveStartDate` | Effective Start Date | string | date |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `memo` | Memo | string |  |  |  |  |
| `name` | Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## bomRevision-componentCollection

Browser definition `bomRevision-componentCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | bomRevision-componentElement[] |  |  | [`bomRevision-componentElement`](#bomrevision-componentelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## bomRevision-componentElement

Browser definition `bomRevision-componentElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `bomQuantity` | BoM Quantity | string |  |  |  |  |
| `componentYield` | Component Yield | number | double |  |  |  |
| `description` | Description | string |  |  |  |  |
| `displayName` | Display Name | string |  |  |  |  |
| `id` | Internal ID | integer | int64 |  |  |  |
| `isOutsourcingCharge` | Is Outsourcing charge | string |  |  |  |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemSource` |  | object |  |  |  |  |
| `itemSource.id` | Internal identifier | string |  |  |  | `WORK_ORDER`, `PHANTOM`, `PURCHASE_ORDER`, `STOCK` |
| `itemSource.refName` | Reference Name | string |  |  |  |  |
| `lineId` | Line Id | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `quantity` | Quantity | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `units` | Units | string |  |  |  |  |

## bomRevisionCollection

Browser definition `bomRevisionCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | bomRevision[] |  |  | [`bomRevision`](#bomrevision) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## bomRevisionSelectOptions

Browser definition `bomRevisionSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `billOfMaterials` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
