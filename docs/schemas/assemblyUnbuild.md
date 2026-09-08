# Schemas: assemblyUnbuild

Property tables for definitions owned by `assemblyUnbuild`.

Record page: [assemblyUnbuild](../records/assemblyUnbuild.md).

## Index

- [assemblyUnbuild](#assemblyunbuild) — 40 properties
- [assemblyUnbuild-accountingBookDetailCollection](#assemblyunbuild-accountingbookdetailcollection) — 6 properties
- [assemblyUnbuild-accountingBookDetailElement](#assemblyunbuild-accountingbookdetailelement) — 7 properties
- [assemblyUnbuild-component-componentInventoryDetail](#assemblyunbuild-component-componentinventorydetail) — 11 properties
- [assemblyUnbuild-component-componentInventoryDetail-inventoryAssignmentCollection](#assemblyunbuild-component-componentinventorydetail-inventoryassignmentcollection) — 6 properties
- [assemblyUnbuild-component-componentInventoryDetail-inventoryAssignmentElement](#assemblyunbuild-component-componentinventorydetail-inventoryassignmentelement) — 17 properties
- [assemblyUnbuild-componentCollection](#assemblyunbuild-componentcollection) — 6 properties
- [assemblyUnbuild-componentElement](#assemblyunbuild-componentelement) — 12 properties
- [assemblyUnbuild-inventoryDetail](#assemblyunbuild-inventorydetail) — 11 properties
- [assemblyUnbuild-inventoryDetail-inventoryAssignmentCollection](#assemblyunbuild-inventorydetail-inventoryassignmentcollection) — 6 properties
- [assemblyUnbuild-inventoryDetail-inventoryAssignmentElement](#assemblyunbuild-inventorydetail-inventoryassignmentelement) — 17 properties
- [assemblyUnbuildCollection](#assemblyunbuildcollection) — 6 properties
- [assemblyUnbuildSelectOptions](#assemblyunbuildselectoptions) — 15 properties

## assemblyUnbuild

Browser definition `assemblyUnbuild`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBookDetail` |  | assemblyUnbuild-accountingBookDetailCollection |  |  | [`assemblyUnbuild-accountingBookDetailCollection`](#assemblyunbuild-accountingbookdetailcollection) |  |
| `billOfMaterials` |  | bom |  |  | [`bom`](bom.md#bom) |  |
| `billOfMaterialsRevision` |  | bomRevision |  |  | [`bomRevision`](bomRevision.md#bomrevision) |  |
| `binNumbers` | Bin Numbers | string |  |  |  |  |
| `built` | Built | number | float |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `component` |  | assemblyUnbuild-componentCollection |  |  | [`assemblyUnbuild-componentCollection`](#assemblyunbuild-componentcollection) |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `createdFrom` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReason` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReasonMemo` | Deletion Reason Memo | string |  |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `effectiveBomControl` | Effective BoM Control | string |  |  |  |  |
| `excludeFromGLNumbering` | Exclude from GL Audit Numbering | boolean |  |  |  |  |
| `expirationDate` | Expiration Date | string | date |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `inventoryDetail` |  | assemblyUnbuild-inventoryDetail |  |  | [`assemblyUnbuild-inventoryDetail`](#assemblyunbuild-inventorydetail) |  |
| `item` |  | assemblyItem |  |  | [`assemblyItem`](assemblyItem.md#assemblyitem) |  |
| `lastModifiedDate` | Date Last Modified | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `outsourcingCharge` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `outsourcingChargeUnitPrice` | Unit Price | number | double |  |  |  |
| `postingPeriod` |  | accountingPeriod |  |  | [`accountingPeriod`](accountingPeriod.md#accountingperiod) |  |
| `prevDate` | Previous Effective Date | string | date |  |  |  |
| `primaryBookBaseCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `quantity` | Quantity | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revision` |  | itemRevision |  |  | [`itemRevision`](itemRevision.md#itemrevision) |  |
| `revisionMemo` | Revision Memo | string |  |  |  |  |
| `serialNumbers` | Serial Numbers | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `total` | Projected Value | number | double |  |  |  |
| `tranDate` | Date | string | date |  |  |  |
| `tranId` | Ref No. | string |  |  |  |  |
| `transactionNumber` | Transaction Number | string |  |  |  |  |
| `units` | Unit of Measure | string |  |  |  |  |

## assemblyUnbuild-accountingBookDetailCollection

Browser definition `assemblyUnbuild-accountingBookDetailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | assemblyUnbuild-accountingBookDetailElement[] |  |  | [`assemblyUnbuild-accountingBookDetailElement`](#assemblyunbuild-accountingbookdetailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## assemblyUnbuild-accountingBookDetailElement

Browser definition `assemblyUnbuild-accountingBookDetailElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | accountingBook |  |  | [`accountingBook`](accountingBook.md#accountingbook) |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revRecOnRevCommitment` | Rev Rec on Rev Commit. | boolean |  |  |  |  |
| `tranIsVsoeBundle` | Transaction Is VSOE Bundle | boolean |  |  |  |  |

## assemblyUnbuild-component-componentInventoryDetail

Browser definition `assemblyUnbuild-component-componentInventoryDetail`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `externalId` | External ID | string |  |  |  |  |
| `inventoryAssignment` |  | assemblyUnbuild-component-componentInventoryDetail-inventoryAssignmentCollection |  |  | [`assemblyUnbuild-component-componentInventoryDetail-inventoryAssignmentCollection`](#assemblyunbuild-component-componentinventorydetail-inventoryassignmentcollection) |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemDescription` | Description | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `quantity` | Quantity | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `toLocation` |  | location |  |  | [`location`](location.md#location) |  |
| `unit` | Units | string |  |  |  |  |

## assemblyUnbuild-component-componentInventoryDetail-inventoryAssignmentCollection

Browser definition `assemblyUnbuild-component-componentInventoryDetail-inventoryAssignmentCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | assemblyUnbuild-component-componentInventoryDetail-inventoryAssignmentElement[] |  |  | [`assemblyUnbuild-component-componentInventoryDetail-inventoryAssignmentElement`](#assemblyunbuild-component-componentinventorydetail-inventoryassignmentelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## assemblyUnbuild-component-componentInventoryDetail-inventoryAssignmentElement

Browser definition `assemblyUnbuild-component-componentInventoryDetail-inventoryAssignmentElement`.

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

## assemblyUnbuild-componentCollection

Browser definition `assemblyUnbuild-componentCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | assemblyUnbuild-componentElement[] |  |  | [`assemblyUnbuild-componentElement`](#assemblyunbuild-componentelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## assemblyUnbuild-componentElement

Browser definition `assemblyUnbuild-componentElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `binNumbers` | Bin Numbers | string |  |  |  |  |
| `buildVariance` | Build Variance | number | float |  |  |  |
| `componentInventoryDetail` |  | assemblyUnbuild-component-componentInventoryDetail |  |  | [`assemblyUnbuild-component-componentInventoryDetail`](#assemblyunbuild-component-componentinventorydetail) |  |
| `componentNumbers` | Serial Numbers | string |  |  |  |  |
| `item` | Item | string |  |  |  |  |
| `lineNumber` | Line Number | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `quantity` | Quantity | number | float |  |  |  |
| `quantityOnHand` | Quantity On Hand | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `unitCost` | Unit Cost | number | float |  |  |  |
| `units` | Units | string |  |  |  |  |

## assemblyUnbuild-inventoryDetail

Browser definition `assemblyUnbuild-inventoryDetail`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `externalId` | External ID | string |  |  |  |  |
| `inventoryAssignment` |  | assemblyUnbuild-inventoryDetail-inventoryAssignmentCollection |  |  | [`assemblyUnbuild-inventoryDetail-inventoryAssignmentCollection`](#assemblyunbuild-inventorydetail-inventoryassignmentcollection) |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemDescription` | Description | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `quantity` | Quantity | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `toLocation` |  | location |  |  | [`location`](location.md#location) |  |
| `unit` | Units | string |  |  |  |  |

## assemblyUnbuild-inventoryDetail-inventoryAssignmentCollection

Browser definition `assemblyUnbuild-inventoryDetail-inventoryAssignmentCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | assemblyUnbuild-inventoryDetail-inventoryAssignmentElement[] |  |  | [`assemblyUnbuild-inventoryDetail-inventoryAssignmentElement`](#assemblyunbuild-inventorydetail-inventoryassignmentelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## assemblyUnbuild-inventoryDetail-inventoryAssignmentElement

Browser definition `assemblyUnbuild-inventoryDetail-inventoryAssignmentElement`.

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

## assemblyUnbuildCollection

Browser definition `assemblyUnbuildCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | assemblyUnbuild[] |  |  | [`assemblyUnbuild`](#assemblyunbuild) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## assemblyUnbuildSelectOptions

Browser definition `assemblyUnbuildSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `billOfMaterials` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billOfMaterialsRevision` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `createdFrom` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deletionReason` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `item` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `outsourcingCharge` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `postingPeriod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `primaryBookBaseCurrency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `revision` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `units` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
