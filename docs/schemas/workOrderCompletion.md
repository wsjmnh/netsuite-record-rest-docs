# Schemas: workOrderCompletion

Property tables for definitions owned by `workOrderCompletion`.

Record page: [workOrderCompletion](../records/workOrderCompletion.md).

## Index

- [workOrderCompletion](#workordercompletion) — 42 properties
- [workOrderCompletion-accountingBookDetailCollection](#workordercompletion-accountingbookdetailcollection) — 6 properties
- [workOrderCompletion-accountingBookDetailElement](#workordercompletion-accountingbookdetailelement) — 7 properties
- [workOrderCompletion-component-componentInventoryDetail](#workordercompletion-component-componentinventorydetail) — 11 properties
- [workOrderCompletion-component-componentInventoryDetail-inventoryAssignmentCollection](#workordercompletion-component-componentinventorydetail-inventoryassignmentcollection) — 6 properties
- [workOrderCompletion-component-componentInventoryDetail-inventoryAssignmentElement](#workordercompletion-component-componentinventorydetail-inventoryassignmentelement) — 17 properties
- [workOrderCompletion-componentCollection](#workordercompletion-componentcollection) — 6 properties
- [workOrderCompletion-componentElement](#workordercompletion-componentelement) — 16 properties
- [workOrderCompletion-inventoryDetail](#workordercompletion-inventorydetail) — 11 properties
- [workOrderCompletion-inventoryDetail-inventoryAssignmentCollection](#workordercompletion-inventorydetail-inventoryassignmentcollection) — 6 properties
- [workOrderCompletion-inventoryDetail-inventoryAssignmentElement](#workordercompletion-inventorydetail-inventoryassignmentelement) — 17 properties
- [workOrderCompletion-operationCollection](#workordercompletion-operationcollection) — 6 properties
- [workOrderCompletion-operationElement](#workordercompletion-operationelement) — 24 properties
- [workOrderCompletionCollection](#workordercompletioncollection) — 6 properties
- [workOrderCompletionSelectOptions](#workordercompletionselectoptions) — 17 properties

## workOrderCompletion

Browser definition `workOrderCompletion`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBookDetail` |  | workOrderCompletion-accountingBookDetailCollection |  |  | [`workOrderCompletion-accountingBookDetailCollection`](#workordercompletion-accountingbookdetailcollection) |  |
| `billOfMaterials` |  | bom |  |  | [`bom`](bom.md#bom) |  |
| `billOfMaterialsRevision` |  | bomRevision |  |  | [`bomRevision`](bomRevision.md#bomrevision) |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `completedQuantity` | Completed Quantity | number | float |  |  |  |
| `component` |  | workOrderCompletion-componentCollection |  |  | [`workOrderCompletion-componentCollection`](#workordercompletion-componentcollection) |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `createdFrom` |  | workOrder |  |  | [`workOrder`](workOrder.md#workorder) |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReason` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReasonMemo` | Deletion Reason Memo | string |  |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `endOperation` |  | manufacturingOperationTask |  |  | [`manufacturingOperationTask`](manufacturingOperationTask.md#manufacturingoperationtask) |  |
| `excludeFromGLNumbering` | Exclude from GL Audit Numbering | boolean |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `inventoryDetail` |  | workOrderCompletion-inventoryDetail |  |  | [`workOrderCompletion-inventoryDetail`](#workordercompletion-inventorydetail) |  |
| `isBackflush` | Backflush | boolean |  |  |  |  |
| `item` |  | assemblyItem |  |  | [`assemblyItem`](assemblyItem.md#assemblyitem) |  |
| `lastModifiedDate` | Date Last Modified | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `manufacturingRouting` |  | manufacturingRouting |  |  | [`manufacturingRouting`](manufacturingRouting.md#manufacturingrouting) |  |
| `memo` | Memo | string |  |  |  |  |
| `operation` |  | workOrderCompletion-operationCollection |  |  | [`workOrderCompletion-operationCollection`](#workordercompletion-operationcollection) |  |
| `orderQuantity` | Work Order Quantity | number | float |  |  |  |
| `postingPeriod` |  | accountingPeriod |  |  | [`accountingPeriod`](accountingPeriod.md#accountingperiod) |  |
| `prevDate` | Previous Effective Date | string | date |  |  |  |
| `primaryBookBaseCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `projectedValue` | Projected Value | number | double |  |  |  |
| `quantity` | Quantity | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revision` |  | itemRevision |  |  | [`itemRevision`](itemRevision.md#itemrevision) |  |
| `revisionMemo` | Revision Memo | string |  |  |  |  |
| `scrapQuantity` | Scrap Quantity | number | float |  |  |  |
| `startOperation` |  | manufacturingOperationTask |  |  | [`manufacturingOperationTask`](manufacturingOperationTask.md#manufacturingoperationtask) |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `total` | Projected Value | number | double |  |  |  |
| `tranDate` | Date | string | date |  |  |  |
| `tranId` | Ref No. | string |  |  |  |  |
| `transactionNumber` | Transaction Number | string |  |  |  |  |
| `units` | Unit of Measure | string |  |  |  |  |

## workOrderCompletion-accountingBookDetailCollection

Browser definition `workOrderCompletion-accountingBookDetailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | workOrderCompletion-accountingBookDetailElement[] |  |  | [`workOrderCompletion-accountingBookDetailElement`](#workordercompletion-accountingbookdetailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## workOrderCompletion-accountingBookDetailElement

Browser definition `workOrderCompletion-accountingBookDetailElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | accountingBook |  |  | [`accountingBook`](accountingBook.md#accountingbook) |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revRecOnRevCommitment` | Rev Rec on Rev Commit. | boolean |  |  |  |  |
| `tranIsVsoeBundle` | Transaction Is VSOE Bundle | boolean |  |  |  |  |

## workOrderCompletion-component-componentInventoryDetail

Browser definition `workOrderCompletion-component-componentInventoryDetail`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `externalId` | External ID | string |  |  |  |  |
| `inventoryAssignment` |  | workOrderCompletion-component-componentInventoryDetail-inventoryAssignmentCollection |  |  | [`workOrderCompletion-component-componentInventoryDetail-inventoryAssignmentCollection`](#workordercompletion-component-componentinventorydetail-inventoryassignmentcollection) |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemDescription` | Description | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `quantity` | Quantity | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `toLocation` |  | location |  |  | [`location`](location.md#location) |  |
| `unit` | Units | string |  |  |  |  |

## workOrderCompletion-component-componentInventoryDetail-inventoryAssignmentCollection

Browser definition `workOrderCompletion-component-componentInventoryDetail-inventoryAssignmentCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | workOrderCompletion-component-componentInventoryDetail-inventoryAssignmentElement[] |  |  | [`workOrderCompletion-component-componentInventoryDetail-inventoryAssignmentElement`](#workordercompletion-component-componentinventorydetail-inventoryassignmentelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## workOrderCompletion-component-componentInventoryDetail-inventoryAssignmentElement

Browser definition `workOrderCompletion-component-componentInventoryDetail-inventoryAssignmentElement`.

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

## workOrderCompletion-componentCollection

Browser definition `workOrderCompletion-componentCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | workOrderCompletion-componentElement[] |  |  | [`workOrderCompletion-componentElement`](#workordercompletion-componentelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## workOrderCompletion-componentElement

Browser definition `workOrderCompletion-componentElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `binNumbers` | Bin Numbers | string |  |  |  |  |
| `compItemName` | Component | string |  |  |  |  |
| `componentInventoryDetail` |  | workOrderCompletion-component-componentInventoryDetail |  |  | [`workOrderCompletion-component-componentInventoryDetail`](#workordercompletion-component-componentinventorydetail) |  |
| `componentNumbers` |  | string |  |  |  |  |
| `isNonInventory` | Non-inventory Item | boolean |  |  |  |  |
| `item` | Item ID | string |  |  |  |  |
| `itemBinList` |  | string |  |  |  |  |
| `lineNumber` | Line Number | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `operationKey` |  | string |  |  |  |  |
| `operationSequenceNumber` | Operation | string |  |  |  |  |
| `operationUrl` |  | string |  |  |  |  |
| `quantity` | Quantity | number | float |  |  |  |
| `quantityPer` | Quantity Per | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `unitCost` | Unit Cost | number | float |  |  |  |

## workOrderCompletion-inventoryDetail

Browser definition `workOrderCompletion-inventoryDetail`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `externalId` | External ID | string |  |  |  |  |
| `inventoryAssignment` |  | workOrderCompletion-inventoryDetail-inventoryAssignmentCollection |  |  | [`workOrderCompletion-inventoryDetail-inventoryAssignmentCollection`](#workordercompletion-inventorydetail-inventoryassignmentcollection) |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemDescription` | Description | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `quantity` | Quantity | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `toLocation` |  | location |  |  | [`location`](location.md#location) |  |
| `unit` | Units | string |  |  |  |  |

## workOrderCompletion-inventoryDetail-inventoryAssignmentCollection

Browser definition `workOrderCompletion-inventoryDetail-inventoryAssignmentCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | workOrderCompletion-inventoryDetail-inventoryAssignmentElement[] |  |  | [`workOrderCompletion-inventoryDetail-inventoryAssignmentElement`](#workordercompletion-inventorydetail-inventoryassignmentelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## workOrderCompletion-inventoryDetail-inventoryAssignmentElement

Browser definition `workOrderCompletion-inventoryDetail-inventoryAssignmentElement`.

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

## workOrderCompletion-operationCollection

Browser definition `workOrderCompletion-operationCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | workOrderCompletion-operationElement[] |  |  | [`workOrderCompletion-operationElement`](#workordercompletion-operationelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## workOrderCompletion-operationElement

Browser definition `workOrderCompletion-operationElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `completedQuantity` | Completed Quantity | number | float |  |  |  |
| `enabled` | Enabled | boolean |  |  |  |  |
| `inputQuantity` | Input Quantity | number | float |  |  |  |
| `laborResources` | Labor Resources | number | float |  |  |  |
| `laborResourcesLimit` | Labor Resources Limit | number | float |  |  |  |
| `laborRunTime` | Labor Run Time (Min) | number | float |  |  |  |
| `laborSetupTime` | Labor Setup Time (Min) | number | float |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `machineResources` | Machine Resources | number | float |  |  |  |
| `machineResourcesLimit` | Machine Resources Limit | number | float |  |  |  |
| `machineRunTime` | Machine Run Time (Min) | number | float |  |  |  |
| `machineSetupTime` | Machine Setup Time (Min) | number | float |  |  |  |
| `operationName` | Operation Name | string |  |  |  |  |
| `operationSequence` | Operation Sequence | integer | int64 |  |  |  |
| `overallCompletedQuantity` | Overall Completed Quantity | number | float |  |  |  |
| `predecessorCompletedQuantity` | Predecessor Completed Quantity | number | float |  |  |  |
| `quantityRemaining` | Quantity Remaining | number | float |  |  |  |
| `recordSetup` | Record Setup Time | boolean |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `runRate` | Run Rate | number | float |  |  |  |
| `setupTime` | Setup Time (Min) | number | float |  |  |  |
| `taskId` | Task Id | integer | int64 |  |  |  |
| `timeId` | Time Id | integer | int64 |  |  |  |
| `workCenter` | Manufacturing Work Center | string |  |  |  |  |

## workOrderCompletionCollection

Browser definition `workOrderCompletionCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | workOrderCompletion[] |  |  | [`workOrderCompletion`](#workordercompletion) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## workOrderCompletionSelectOptions

Browser definition `workOrderCompletionSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `billOfMaterials` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billOfMaterialsRevision` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `createdFrom` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deletionReason` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `endOperation` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `item` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `manufacturingRouting` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `postingPeriod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `primaryBookBaseCurrency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `revision` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `startOperation` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `units` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
