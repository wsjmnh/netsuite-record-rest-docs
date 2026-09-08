# Schemas: workOrderIssue

Property tables for definitions owned by `workOrderIssue`.

Record page: [workOrderIssue](../records/workOrderIssue.md).

## Index

- [workOrderIssue](#workorderissue) — 30 properties
- [workOrderIssue-component-componentInventoryDetail](#workorderissue-component-componentinventorydetail) — 11 properties
- [workOrderIssue-component-componentInventoryDetail-inventoryAssignmentCollection](#workorderissue-component-componentinventorydetail-inventoryassignmentcollection) — 6 properties
- [workOrderIssue-component-componentInventoryDetail-inventoryAssignmentElement](#workorderissue-component-componentinventorydetail-inventoryassignmentelement) — 17 properties
- [workOrderIssue-componentCollection](#workorderissue-componentcollection) — 6 properties
- [workOrderIssue-componentElement](#workorderissue-componentelement) — 15 properties
- [workOrderIssueCollection](#workorderissuecollection) — 6 properties
- [workOrderIssueSelectOptions](#workorderissueselectoptions) — 15 properties

## workOrderIssue

Browser definition `workOrderIssue`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `billOfMaterials` |  | bom |  |  | [`bom`](bom.md#bom) |  |
| `billOfMaterialsRevision` |  | bomRevision |  |  | [`bomRevision`](bomRevision.md#bomrevision) |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `component` |  | workOrderIssue-componentCollection |  |  | [`workOrderIssue-componentCollection`](#workorderissue-componentcollection) |  |
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
| `item` |  | assemblyItem |  |  | [`assemblyItem`](assemblyItem.md#assemblyitem) |  |
| `lastModifiedDate` | Date Last Modified | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `manufacturingRouting` |  | manufacturingRouting |  |  | [`manufacturingRouting`](manufacturingRouting.md#manufacturingrouting) |  |
| `memo` | Memo | string |  |  |  |  |
| `postingPeriod` |  | accountingPeriod |  |  | [`accountingPeriod`](accountingPeriod.md#accountingperiod) |  |
| `prevDate` | Previous Effective Date | string | date |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revision` |  | itemRevision |  |  | [`itemRevision`](itemRevision.md#itemrevision) |  |
| `revisionMemo` | Revision Memo | string |  |  |  |  |
| `startOperation` |  | manufacturingOperationTask |  |  | [`manufacturingOperationTask`](manufacturingOperationTask.md#manufacturingoperationtask) |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `tranDate` | Date | string | date |  |  |  |
| `tranId` | Ref No. | string |  |  |  |  |
| `transactionNumber` | Transaction Number | string |  |  |  |  |

## workOrderIssue-component-componentInventoryDetail

Browser definition `workOrderIssue-component-componentInventoryDetail`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `externalId` | External ID | string |  |  |  |  |
| `inventoryAssignment` |  | workOrderIssue-component-componentInventoryDetail-inventoryAssignmentCollection |  |  | [`workOrderIssue-component-componentInventoryDetail-inventoryAssignmentCollection`](#workorderissue-component-componentinventorydetail-inventoryassignmentcollection) |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemDescription` | Description | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `quantity` | Quantity | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `toLocation` |  | location |  |  | [`location`](location.md#location) |  |
| `unit` | Units | string |  |  |  |  |

## workOrderIssue-component-componentInventoryDetail-inventoryAssignmentCollection

Browser definition `workOrderIssue-component-componentInventoryDetail-inventoryAssignmentCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | workOrderIssue-component-componentInventoryDetail-inventoryAssignmentElement[] |  |  | [`workOrderIssue-component-componentInventoryDetail-inventoryAssignmentElement`](#workorderissue-component-componentinventorydetail-inventoryassignmentelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## workOrderIssue-component-componentInventoryDetail-inventoryAssignmentElement

Browser definition `workOrderIssue-component-componentInventoryDetail-inventoryAssignmentElement`.

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

## workOrderIssue-componentCollection

Browser definition `workOrderIssue-componentCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | workOrderIssue-componentElement[] |  |  | [`workOrderIssue-componentElement`](#workorderissue-componentelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## workOrderIssue-componentElement

Browser definition `workOrderIssue-componentElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `binNumbers` | Bin Numbers | string |  |  |  |  |
| `compItemName` | Component | string |  |  |  |  |
| `componentInventoryDetail` |  | workOrderIssue-component-componentInventoryDetail |  |  | [`workOrderIssue-component-componentInventoryDetail`](#workorderissue-component-componentinventorydetail) |  |
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
| `refName` | Reference Name | string |  |  |  |  |
| `unitCost` | Unit Cost | number | float |  |  |  |

## workOrderIssueCollection

Browser definition `workOrderIssueCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | workOrderIssue[] |  |  | [`workOrderIssue`](#workorderissue) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## workOrderIssueSelectOptions

Browser definition `workOrderIssueSelectOptions`.

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
| `revision` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `startOperation` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
