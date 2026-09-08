# Schemas: assemblyBuild

Property tables for definitions owned by `assemblyBuild`.

Record page: [assemblyBuild](../records/assemblyBuild.md).

## Index

- [assemblyBuild](#assemblybuild) — 43 properties
- [assemblyBuild-accountingBookDetailCollection](#assemblybuild-accountingbookdetailcollection) — 6 properties
- [assemblyBuild-accountingBookDetailElement](#assemblybuild-accountingbookdetailelement) — 7 properties
- [assemblyBuild-component-componentInventoryDetail](#assemblybuild-component-componentinventorydetail) — 11 properties
- [assemblyBuild-component-componentInventoryDetail-inventoryAssignmentCollection](#assemblybuild-component-componentinventorydetail-inventoryassignmentcollection) — 6 properties
- [assemblyBuild-component-componentInventoryDetail-inventoryAssignmentElement](#assemblybuild-component-componentinventorydetail-inventoryassignmentelement) — 17 properties
- [assemblyBuild-componentCollection](#assemblybuild-componentcollection) — 6 properties
- [assemblyBuild-componentElement](#assemblybuild-componentelement) — 12 properties
- [assemblyBuild-inventoryDetail](#assemblybuild-inventorydetail) — 11 properties
- [assemblyBuild-inventoryDetail-inventoryAssignmentCollection](#assemblybuild-inventorydetail-inventoryassignmentcollection) — 6 properties
- [assemblyBuild-inventoryDetail-inventoryAssignmentElement](#assemblybuild-inventorydetail-inventoryassignmentelement) — 17 properties
- [assemblyBuildCollection](#assemblybuildcollection) — 6 properties
- [assemblyBuildSelectOptions](#assemblybuildselectoptions) — 17 properties

## assemblyBuild

Browser definition `assemblyBuild`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBookDetail` |  | assemblyBuild-accountingBookDetailCollection |  |  | [`assemblyBuild-accountingBookDetailCollection`](#assemblybuild-accountingbookdetailcollection) |  |
| `billOfMaterials` |  | bom |  |  | [`bom`](bom.md#bom) |  |
| `billOfMaterialsRevision` |  | bomRevision |  |  | [`bomRevision`](bomRevision.md#bomrevision) |  |
| `binNumbers` | Bin Numbers | string |  |  |  |  |
| `buildable` | Buildable | number | float |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `component` |  | assemblyBuild-componentCollection |  |  | [`assemblyBuild-componentCollection`](#assemblybuild-componentcollection) |  |
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
| `inventoryDetail` |  | assemblyBuild-inventoryDetail |  |  | [`assemblyBuild-inventoryDetail`](#assemblybuild-inventorydetail) |  |
| `item` |  | assemblyItem |  |  | [`assemblyItem`](assemblyItem.md#assemblyitem) |  |
| `lastModifiedDate` | Date Last Modified | string | date-time |  |  |  |
| `linkedIR` |  | itemReceipt |  |  | [`itemReceipt`](itemReceipt.md#itemreceipt) |  |
| `linkedInventoryTransfer` |  | inventoryTransfer |  |  | [`inventoryTransfer`](inventoryTransfer.md#inventorytransfer) |  |
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
| `unbuilt` | Unbuilt | number | float |  |  |  |
| `units` | Unit of Measure | string |  |  |  |  |

## assemblyBuild-accountingBookDetailCollection

Browser definition `assemblyBuild-accountingBookDetailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | assemblyBuild-accountingBookDetailElement[] |  |  | [`assemblyBuild-accountingBookDetailElement`](#assemblybuild-accountingbookdetailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## assemblyBuild-accountingBookDetailElement

Browser definition `assemblyBuild-accountingBookDetailElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | accountingBook |  |  | [`accountingBook`](accountingBook.md#accountingbook) |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revRecOnRevCommitment` | Rev Rec on Rev Commit. | boolean |  |  |  |  |
| `tranIsVsoeBundle` | Transaction Is VSOE Bundle | boolean |  |  |  |  |

## assemblyBuild-component-componentInventoryDetail

Browser definition `assemblyBuild-component-componentInventoryDetail`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `externalId` | External ID | string |  |  |  |  |
| `inventoryAssignment` |  | assemblyBuild-component-componentInventoryDetail-inventoryAssignmentCollection |  |  | [`assemblyBuild-component-componentInventoryDetail-inventoryAssignmentCollection`](#assemblybuild-component-componentinventorydetail-inventoryassignmentcollection) |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemDescription` | Description | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `quantity` | Quantity | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `toLocation` |  | location |  |  | [`location`](location.md#location) |  |
| `unit` | Units | string |  |  |  |  |

## assemblyBuild-component-componentInventoryDetail-inventoryAssignmentCollection

Browser definition `assemblyBuild-component-componentInventoryDetail-inventoryAssignmentCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | assemblyBuild-component-componentInventoryDetail-inventoryAssignmentElement[] |  |  | [`assemblyBuild-component-componentInventoryDetail-inventoryAssignmentElement`](#assemblybuild-component-componentinventorydetail-inventoryassignmentelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## assemblyBuild-component-componentInventoryDetail-inventoryAssignmentElement

Browser definition `assemblyBuild-component-componentInventoryDetail-inventoryAssignmentElement`.

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

## assemblyBuild-componentCollection

Browser definition `assemblyBuild-componentCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | assemblyBuild-componentElement[] |  |  | [`assemblyBuild-componentElement`](#assemblybuild-componentelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## assemblyBuild-componentElement

Browser definition `assemblyBuild-componentElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `binNumbers` | Bin Numbers | string |  |  |  |  |
| `buildVariance` | Build Variance | number | float |  |  |  |
| `componentInventoryDetail` |  | assemblyBuild-component-componentInventoryDetail |  |  | [`assemblyBuild-component-componentInventoryDetail`](#assemblybuild-component-componentinventorydetail) |  |
| `componentNumbers` | Serial Numbers | string |  |  |  |  |
| `item` | Item | string |  |  |  |  |
| `lineNumber` | Line Number | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `quantity` | Quantity | number | float |  |  |  |
| `quantityOnHand` | Quantity On Hand | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `unitCost` | Unit Cost | number | float |  |  |  |
| `units` | Units | string |  |  |  |  |

## assemblyBuild-inventoryDetail

Browser definition `assemblyBuild-inventoryDetail`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `externalId` | External ID | string |  |  |  |  |
| `inventoryAssignment` |  | assemblyBuild-inventoryDetail-inventoryAssignmentCollection |  |  | [`assemblyBuild-inventoryDetail-inventoryAssignmentCollection`](#assemblybuild-inventorydetail-inventoryassignmentcollection) |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemDescription` | Description | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `quantity` | Quantity | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `toLocation` |  | location |  |  | [`location`](location.md#location) |  |
| `unit` | Units | string |  |  |  |  |

## assemblyBuild-inventoryDetail-inventoryAssignmentCollection

Browser definition `assemblyBuild-inventoryDetail-inventoryAssignmentCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | assemblyBuild-inventoryDetail-inventoryAssignmentElement[] |  |  | [`assemblyBuild-inventoryDetail-inventoryAssignmentElement`](#assemblybuild-inventorydetail-inventoryassignmentelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## assemblyBuild-inventoryDetail-inventoryAssignmentElement

Browser definition `assemblyBuild-inventoryDetail-inventoryAssignmentElement`.

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

## assemblyBuildCollection

Browser definition `assemblyBuildCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | assemblyBuild[] |  |  | [`assemblyBuild`](#assemblybuild) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## assemblyBuildSelectOptions

Browser definition `assemblyBuildSelectOptions`.

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
| `linkedIR` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `linkedInventoryTransfer` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `outsourcingCharge` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `postingPeriod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `primaryBookBaseCurrency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `revision` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `units` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
