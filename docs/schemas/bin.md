# Schemas: bin

Property tables for definitions owned by `bin`.

Record page: [bin](../records/bin.md).

## Index

- [bin](#bin) — 16 properties
- [bin-inventoryBalanceCollection](#bin-inventorybalancecollection) — 6 properties
- [bin-inventoryBalanceElement](#bin-inventorybalanceelement) — 15 properties
- [binCollection](#bincollection) — 6 properties
- [binSelectOptions](#binselectoptions) — 3 properties

## bin

Browser definition `bin`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `binNumber` | Bin Number | string |  |  |  |  |
| `blockFromWaveOrderPicking` | Block from Wave Order Picking | boolean |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `inventoryBalance` |  | bin-inventoryBalanceCollection |  |  | [`bin-inventoryBalanceCollection`](#bin-inventorybalancecollection) |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `sequenceNumber` | Sequence Number | number | float |  |  |  |
| `type` |  | object |  |  |  |  |
| `type.id` | Internal identifier | string |  |  |  | `OUTBOUND_STAGING`, `STORAGE`, `VENDOR_RETURNS`, `PICKING`, `INBOUND_STAGING`, `NONE`, `WIP` |
| `type.refName` | Reference Name | string |  |  |  |  |
| `zone` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |

## bin-inventoryBalanceCollection

Browser definition `bin-inventoryBalanceCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | bin-inventoryBalanceElement[] |  |  | [`bin-inventoryBalanceElement`](#bin-inventorybalanceelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## bin-inventoryBalanceElement

Browser definition `bin-inventoryBalanceElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `committedQtyPerLocation` | Committed Quantity (Per Location) | string |  |  |  |  |
| `committedQtyPerSerialLotNumber` | Committed Quantity (Per Serial/Lot Number) | string |  |  |  |  |
| `committedQtyPerSerialLotNumberLocation` | Committed Quantity (Per Serial/Lot Number & Location) | string |  |  |  |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `inventoryNumber` |  | inventoryNumber |  |  | [`inventoryNumber`](inventoryNumber.md#inventorynumber) |  |
| `inventoryStatus` |  | inventoryStatus |  |  | [`inventoryStatus`](inventoryStatus.md#inventorystatus) |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `licensePlateNumber` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `quantityAvailable` | Available Quantity | string |  |  |  |  |
| `quantityOnHand` | On-Hand Quantity | string |  |  |  |  |
| `quantityPicked` | Picked Quantity | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## binCollection

Browser definition `binCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | bin[] |  |  | [`bin`](#bin) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## binSelectOptions

Browser definition `binSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `type` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `zone` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
