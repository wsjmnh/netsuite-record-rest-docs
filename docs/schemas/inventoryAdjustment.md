# Schemas: inventoryAdjustment

Property tables for definitions owned by `inventoryAdjustment`.

Record page: [inventoryAdjustment](../records/inventoryAdjustment.md).

## Index

- [inventoryAdjustment](#inventoryadjustment) — 29 properties
- [inventoryAdjustment-accountingBookDetailCollection](#inventoryadjustment-accountingbookdetailcollection) — 6 properties
- [inventoryAdjustment-accountingBookDetailElement](#inventoryadjustment-accountingbookdetailelement) — 7 properties
- [inventoryAdjustment-inventory-inventoryDetail](#inventoryadjustment-inventory-inventorydetail) — 11 properties
- [inventoryAdjustment-inventory-inventoryDetail-inventoryAssignmentCollection](#inventoryadjustment-inventory-inventorydetail-inventoryassignmentcollection) — 6 properties
- [inventoryAdjustment-inventory-inventoryDetail-inventoryAssignmentElement](#inventoryadjustment-inventory-inventorydetail-inventoryassignmentelement) — 17 properties
- [inventoryAdjustment-inventoryCollection](#inventoryadjustment-inventorycollection) — 6 properties
- [inventoryAdjustment-inventoryElement](#inventoryadjustment-inventoryelement) — 29 properties
- [inventoryAdjustmentCollection](#inventoryadjustmentcollection) — 6 properties
- [inventoryAdjustmentSelectOptions](#inventoryadjustmentselectoptions) — 11 properties

## inventoryAdjustment

Browser definition `inventoryAdjustment`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | account |  |  | [`account`](account.md#account) |  |
| `accountingBookDetail` |  | inventoryAdjustment-accountingBookDetailCollection |  |  | [`inventoryAdjustment-accountingBookDetailCollection`](#inventoryadjustment-accountingbookdetailcollection) |  |
| `adjLocation` |  | location |  |  | [`location`](location.md#location) |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `cleared` | Cleared | boolean |  |  |  |  |
| `clearedDate` | Date Cleared | string | date |  |  |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `customer` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `deletionReason` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReasonMemo` | Deletion Reason Memo | string |  |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `estimatedTotalValue` | Estimated Total Value | number | double |  |  |  |
| `excludeFromGLNumbering` | Exclude from GL Audit Numbering | boolean |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `inventory` |  | inventoryAdjustment-inventoryCollection |  |  | [`inventoryAdjustment-inventoryCollection`](#inventoryadjustment-inventorycollection) |  |
| `lastModifiedDate` | Date Last Modified | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `postingPeriod` |  | accountingPeriod |  |  | [`accountingPeriod`](accountingPeriod.md#accountingperiod) |  |
| `prevDate` | Previous Effective Date | string | date |  |  |  |
| `primaryBookBaseCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `tranDate` | Date | string | date |  |  |  |
| `tranId` | Ref No. | string |  |  |  |  |
| `transactionNumber` | Transaction Number | string |  |  |  |  |

## inventoryAdjustment-accountingBookDetailCollection

Browser definition `inventoryAdjustment-accountingBookDetailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | inventoryAdjustment-accountingBookDetailElement[] |  |  | [`inventoryAdjustment-accountingBookDetailElement`](#inventoryadjustment-accountingbookdetailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## inventoryAdjustment-accountingBookDetailElement

Browser definition `inventoryAdjustment-accountingBookDetailElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | accountingBook |  |  | [`accountingBook`](accountingBook.md#accountingbook) |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revRecOnRevCommitment` | Rev Rec on Rev Commit. | boolean |  |  |  |  |
| `tranIsVsoeBundle` | Transaction Is VSOE Bundle | boolean |  |  |  |  |

## inventoryAdjustment-inventory-inventoryDetail

Browser definition `inventoryAdjustment-inventory-inventoryDetail`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `externalId` | External ID | string |  |  |  |  |
| `inventoryAssignment` |  | inventoryAdjustment-inventory-inventoryDetail-inventoryAssignmentCollection |  |  | [`inventoryAdjustment-inventory-inventoryDetail-inventoryAssignmentCollection`](#inventoryadjustment-inventory-inventorydetail-inventoryassignmentcollection) |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemDescription` | Description | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `quantity` | Quantity | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `toLocation` |  | location |  |  | [`location`](location.md#location) |  |
| `unit` | Units | string |  |  |  |  |

## inventoryAdjustment-inventory-inventoryDetail-inventoryAssignmentCollection

Browser definition `inventoryAdjustment-inventory-inventoryDetail-inventoryAssignmentCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | inventoryAdjustment-inventory-inventoryDetail-inventoryAssignmentElement[] |  |  | [`inventoryAdjustment-inventory-inventoryDetail-inventoryAssignmentElement`](#inventoryadjustment-inventory-inventorydetail-inventoryassignmentelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## inventoryAdjustment-inventory-inventoryDetail-inventoryAssignmentElement

Browser definition `inventoryAdjustment-inventory-inventoryDetail-inventoryAssignmentElement`.

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

## inventoryAdjustment-inventoryCollection

Browser definition `inventoryAdjustment-inventoryCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | inventoryAdjustment-inventoryElement[] |  |  | [`inventoryAdjustment-inventoryElement`](#inventoryadjustment-inventoryelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## inventoryAdjustment-inventoryElement

Browser definition `inventoryAdjustment-inventoryElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `adjustQtyBy` | Adjust Qty By | number | float |  |  |  |
| `binNumbers` | Bin Numbers | string |  |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `costingMethod` |  | object |  |  |  |  |
| `costingMethod.id` | Internal identifier | string |  |  |  | `SERIAL`, `LOT`, `AVG`, `LIFO`, `GROUPAVG`, `FIFO`, `STANDARD` |
| `costingMethod.refName` | Reference Name | string |  |  |  |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `currentValue` | Current Value | number | double |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `description` | Description | string |  |  |  |  |
| `exchangeRate` | Exchange Rate | number | float |  |  |  |
| `expirationDate` | Expiration Date | string | date |  |  |  |
| `foreignCurrencyUnitCost` | Unit Cost | number | double |  |  |  |
| `inventoryDetail` |  | inventoryAdjustment-inventory-inventoryDetail |  |  | [`inventoryAdjustment-inventory-inventoryDetail`](#inventoryadjustment-inventory-inventorydetail) |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `label` | Exchange Rate | string |  |  |  |  |
| `labelCurrency` | Currency | string |  |  |  |  |
| `labelFxUnitCost` | Unit Cost in Foreign Currency | string |  |  |  |  |
| `line` | Line | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `newQuantity` | New Qty | number | float |  |  |  |
| `quantityOnHand` | Qty On Hand | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `serialNumbers` | Serial Numbers | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `unitCost` | Unit Cost | number | double |  |  |  |
| `units` | Units | string |  |  |  |  |

## inventoryAdjustmentCollection

Browser definition `inventoryAdjustmentCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | inventoryAdjustment[] |  |  | [`inventoryAdjustment`](#inventoryadjustment) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## inventoryAdjustmentSelectOptions

Browser definition `inventoryAdjustmentSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `adjLocation` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customer` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deletionReason` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `postingPeriod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `primaryBookBaseCurrency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
