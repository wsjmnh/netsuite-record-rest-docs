# Schemas: binTransfer

Property tables for definitions owned by `binTransfer`.

Record page: [binTransfer](../records/binTransfer.md).

## Index

- [binTransfer](#bintransfer) — 16 properties
- [binTransfer-inventory-inventoryDetail](#bintransfer-inventory-inventorydetail) — 11 properties
- [binTransfer-inventory-inventoryDetail-inventoryAssignmentCollection](#bintransfer-inventory-inventorydetail-inventoryassignmentcollection) — 6 properties
- [binTransfer-inventory-inventoryDetail-inventoryAssignmentElement](#bintransfer-inventory-inventorydetail-inventoryassignmentelement) — 17 properties
- [binTransfer-inventoryCollection](#bintransfer-inventorycollection) — 6 properties
- [binTransfer-inventoryElement](#bintransfer-inventoryelement) — 11 properties
- [binTransferCollection](#bintransfercollection) — 6 properties
- [binTransferSelectOptions](#bintransferselectoptions) — 3 properties

## binTransfer

Browser definition `binTransfer`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `deletionReason` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReasonMemo` | Deletion Reason Memo | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `inventory` |  | binTransfer-inventoryCollection |  |  | [`binTransfer-inventoryCollection`](#bintransfer-inventorycollection) |  |
| `lastModifiedDate` | Date Last Modified | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `prevDate` | Previous Effective Date | string | date |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `tranDate` | Date | string | date |  |  |  |
| `tranId` | Bin Transfer # | string |  |  |  |  |
| `transactionNumber` | Transaction Number | string |  |  |  |  |

## binTransfer-inventory-inventoryDetail

Browser definition `binTransfer-inventory-inventoryDetail`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `externalId` | External ID | string |  |  |  |  |
| `inventoryAssignment` |  | binTransfer-inventory-inventoryDetail-inventoryAssignmentCollection |  |  | [`binTransfer-inventory-inventoryDetail-inventoryAssignmentCollection`](#bintransfer-inventory-inventorydetail-inventoryassignmentcollection) |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemDescription` | Description | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `quantity` | Quantity | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `toLocation` |  | location |  |  | [`location`](location.md#location) |  |
| `unit` | Units | string |  |  |  |  |

## binTransfer-inventory-inventoryDetail-inventoryAssignmentCollection

Browser definition `binTransfer-inventory-inventoryDetail-inventoryAssignmentCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | binTransfer-inventory-inventoryDetail-inventoryAssignmentElement[] |  |  | [`binTransfer-inventory-inventoryDetail-inventoryAssignmentElement`](#bintransfer-inventory-inventorydetail-inventoryassignmentelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## binTransfer-inventory-inventoryDetail-inventoryAssignmentElement

Browser definition `binTransfer-inventory-inventoryDetail-inventoryAssignmentElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `binNumber` |  | bin |  |  | [`bin`](bin.md#bin) |  |
| `expirationDate` | Expiration Date | string | date |  |  |  |
| `internalId` | Internal ID | integer | int64 |  |  |  |
| `inventoryDetail` | Inventory Detail | integer | int64 |  |  |  |
| `inventoryStatus` |  | inventoryStatus |  |  | [`inventoryStatus`](inventoryStatus.md#inventorystatus) |  |
| `issueInventoryNumber` |  | inventoryNumber |  |  | [`inventoryNumber`](inventoryNumber.md#inventorynumber) |  |
| `licensePlateNumber` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `packCarton` | Pack Carton | string |  |  |  |  |
| `pickCarton` | Pick Carton | string |  |  |  |  |
| `quantity` | Quantity | number | float |  |  |  |
| `quantityAvailable` | Unpicked Bin Qty | number | float |  |  |  |
| `receiptInventoryNumber` | Serial/Lot Number | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `secondaryQuantity` | Secondary Quantity | number | float |  |  |  |
| `toBinNumber` |  | bin |  |  | [`bin`](bin.md#bin) |  |
| `toInventoryStatus` |  | inventoryStatus |  |  | [`inventoryStatus`](inventoryStatus.md#inventorystatus) |  |

## binTransfer-inventoryCollection

Browser definition `binTransfer-inventoryCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | binTransfer-inventoryElement[] |  |  | [`binTransfer-inventoryElement`](#bintransfer-inventoryelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## binTransfer-inventoryElement

Browser definition `binTransfer-inventoryElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `description` | Description | string |  |  |  |  |
| `fromBins` | From Bins | string |  |  |  |  |
| `inventoryDetail` |  | binTransfer-inventory-inventoryDetail |  |  | [`binTransfer-inventory-inventoryDetail`](#bintransfer-inventory-inventorydetail) |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemUnits` | Units | string |  |  |  |  |
| `line` | Transaction Line | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `preferredBin` | Preferred Bin | string |  |  |  |  |
| `quantity` | Quantity | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `toBins` | To Bins | string |  |  |  |  |

## binTransferCollection

Browser definition `binTransferCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | binTransfer[] |  |  | [`binTransfer`](#bintransfer) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## binTransferSelectOptions

Browser definition `binTransferSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `deletionReason` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
