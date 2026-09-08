# Schemas: binWorksheet

Property tables for definitions owned by `binWorksheet`.

Record page: [binWorksheet](../records/binWorksheet.md).

## Index

- [binWorksheet](#binworksheet) — 16 properties
- [binWorksheet-item-inventoryDetail](#binworksheet-item-inventorydetail) — 11 properties
- [binWorksheet-item-inventoryDetail-inventoryAssignmentCollection](#binworksheet-item-inventorydetail-inventoryassignmentcollection) — 6 properties
- [binWorksheet-item-inventoryDetail-inventoryAssignmentElement](#binworksheet-item-inventorydetail-inventoryassignmentelement) — 17 properties
- [binWorksheet-itemCollection](#binworksheet-itemcollection) — 6 properties
- [binWorksheet-itemElement](#binworksheet-itemelement) — 16 properties
- [binWorksheetCollection](#binworksheetcollection) — 6 properties
- [binWorksheetSelectOptions](#binworksheetselectoptions) — 3 properties

## binWorksheet

Browser definition `binWorksheet`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `deletionReason` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReasonMemo` | Deletion Reason Memo | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `item` |  | binWorksheet-itemCollection |  |  | [`binWorksheet-itemCollection`](#binworksheet-itemcollection) |  |
| `lastModifiedDate` | Date Last Modified | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `prevDate` | Previous Effective Date | string | date |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `tranDate` | Date | string | date |  |  |  |
| `tranId` | Bin Worksheet # | string |  |  |  |  |
| `transactionNumber` | Transaction Number | string |  |  |  |  |

## binWorksheet-item-inventoryDetail

Browser definition `binWorksheet-item-inventoryDetail`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `externalId` | External ID | string |  |  |  |  |
| `inventoryAssignment` |  | binWorksheet-item-inventoryDetail-inventoryAssignmentCollection |  |  | [`binWorksheet-item-inventoryDetail-inventoryAssignmentCollection`](#binworksheet-item-inventorydetail-inventoryassignmentcollection) |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemDescription` | Description | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `quantity` | Quantity | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `toLocation` |  | location |  |  | [`location`](location.md#location) |  |
| `unit` | Units | string |  |  |  |  |

## binWorksheet-item-inventoryDetail-inventoryAssignmentCollection

Browser definition `binWorksheet-item-inventoryDetail-inventoryAssignmentCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | binWorksheet-item-inventoryDetail-inventoryAssignmentElement[] |  |  | [`binWorksheet-item-inventoryDetail-inventoryAssignmentElement`](#binworksheet-item-inventorydetail-inventoryassignmentelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## binWorksheet-item-inventoryDetail-inventoryAssignmentElement

Browser definition `binWorksheet-item-inventoryDetail-inventoryAssignmentElement`.

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

## binWorksheet-itemCollection

Browser definition `binWorksheet-itemCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | binWorksheet-itemElement[] |  |  | [`binWorksheet-itemElement`](#binworksheet-itemelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## binWorksheet-itemElement

Browser definition `binWorksheet-itemElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `baseuomquantity` | Quantity (Base Unit) | number | float |  |  |  |
| `conversionrate` | Conversion Rate {1} | number | float |  |  |  |
| `description` | Description | string |  |  |  |  |
| `inventoryDetail` |  | binWorksheet-item-inventoryDetail |  |  | [`binWorksheet-item-inventoryDetail`](#binworksheet-item-inventorydetail) |  |
| `item` | Item ID | string |  |  |  |  |
| `itemBinNumbers` | Bin Numbers | string |  |  |  |  |
| `itemBins` | Bins | string |  |  |  |  |
| `itemName` | Item | string |  |  |  |  |
| `itemOnHand` | Total | number | float |  |  |  |
| `itemPreferBin` |  | bin |  |  | [`bin`](bin.md#bin) |  |
| `itemUnitsLabel` | Unit Plural Abbreviation | string |  |  |  |  |
| `itemunits` | Units | string |  |  |  |  |
| `line` | Line | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `quantity` | Quantity | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## binWorksheetCollection

Browser definition `binWorksheetCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | binWorksheet[] |  |  | [`binWorksheet`](#binworksheet) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## binWorksheetSelectOptions

Browser definition `binWorksheetSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `deletionReason` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
