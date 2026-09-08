# Schemas: inventoryNumber

Property tables for definitions owned by `inventoryNumber`.

Record page: [inventoryNumber](../records/inventoryNumber.md).

## Index

- [inventoryNumber](#inventorynumber) — 21 properties
- [inventoryNumber-inventoryBalanceCollection](#inventorynumber-inventorybalancecollection) — 6 properties
- [inventoryNumber-inventoryBalanceElement](#inventorynumber-inventorybalanceelement) — 15 properties
- [inventoryNumber-locationsCollection](#inventorynumber-locationscollection) — 6 properties
- [inventoryNumber-locationsElement](#inventorynumber-locationselement) — 11 properties
- [inventoryNumberCollection](#inventorynumbercollection) — 6 properties
- [inventoryNumberSelectOptions](#inventorynumberselectoptions) — 3 properties

## inventoryNumber

Browser definition `inventoryNumber`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `baseUnit` | Base Unit | string |  |  |  |  |
| `expirationDate` | Expiration Date | string | date |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `inventoryBalance` |  | inventoryNumber-inventoryBalanceCollection |  |  | [`inventoryNumber-inventoryBalanceCollection`](#inventorynumber-inventorybalancecollection) |  |
| `inventoryNumber` | Serial/Lot Number | string |  |  |  |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemName` | Item Name | string |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `locations` |  | inventoryNumber-locationsCollection |  |  | [`inventoryNumber-locationsCollection`](#inventorynumber-locationscollection) |  |
| `memo` | Memo | string |  |  |  |  |
| `quantityAvailable` | Available | number | float |  |  |  |
| `quantityAvailableBase` | Available (Base Unit) | number | float |  |  |  |
| `quantityInTransit` | In Transit | number | float |  |  |  |
| `quantityOnHand` | On Hand | number | float |  |  |  |
| `quantityOnHandBase` | On Hand (Base Unit) | number | float |  |  |  |
| `quantityOnOrder` | On Order | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `status` | Status | string |  |  |  |  |
| `units` | Stock Unit | string |  |  |  |  |

## inventoryNumber-inventoryBalanceCollection

Browser definition `inventoryNumber-inventoryBalanceCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | inventoryNumber-inventoryBalanceElement[] |  |  | [`inventoryNumber-inventoryBalanceElement`](#inventorynumber-inventorybalanceelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## inventoryNumber-inventoryBalanceElement

Browser definition `inventoryNumber-inventoryBalanceElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `binNumber` |  | bin |  |  | [`bin`](bin.md#bin) |  |
| `committedQtyPerLocation` | Committed Quantity (Per Location) | string |  |  |  |  |
| `committedQtyPerSerialLotNumber` | Committed Quantity (Per Serial/Lot Number) | string |  |  |  |  |
| `committedQtyPerSerialLotNumberLocation` | Committed Quantity (Per Serial/Lot Number & Location) | string |  |  |  |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
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

## inventoryNumber-locationsCollection

Browser definition `inventoryNumber-locationsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | inventoryNumber-locationsElement[] |  |  | [`inventoryNumber-locationsElement`](#inventorynumber-locationselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## inventoryNumber-locationsElement

Browser definition `inventoryNumber-locationsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `quantityAvailable` | Available | number | float |  |  |  |
| `quantityAvailableBase` | Available (Base Unit) | number | float |  |  |  |
| `quantityInTransit` | In Transit | number | float |  |  |  |
| `quantityOnHand` | On Hand | number | float |  |  |  |
| `quantityOnHandBase` | On Hand (Base Unit) | number | float |  |  |  |
| `quantityOnOrder` | On Order | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## inventoryNumberCollection

Browser definition `inventoryNumberCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | inventoryNumber[] |  |  | [`inventoryNumber`](#inventorynumber) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## inventoryNumberSelectOptions

Browser definition `inventoryNumberSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `baseUnit` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `item` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `units` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
