# Schemas: workOrderClose

Property tables for definitions owned by `workOrderClose`.

Record page: [workOrderClose](../records/workOrderClose.md).

## Index

- [workOrderClose](#workorderclose) — 35 properties
- [workOrderClose-componentCollection](#workorderclose-componentcollection) — 6 properties
- [workOrderClose-componentElement](#workorderclose-componentelement) — 9 properties
- [workOrderClose-routingItemCollection](#workorderclose-routingitemcollection) — 6 properties
- [workOrderClose-routingItemElement](#workorderclose-routingitemelement) — 14 properties
- [workOrderCloseCollection](#workorderclosecollection) — 6 properties
- [workOrderCloseSelectOptions](#workordercloseselectoptions) — 12 properties

## workOrderClose

Browser definition `workOrderClose`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `billOfMaterials` |  | bom |  |  | [`bom`](bom.md#bom) |  |
| `billOfMaterialsRevision` |  | bomRevision |  |  | [`bomRevision`](bomRevision.md#bomrevision) |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `component` |  | workOrderClose-componentCollection |  |  | [`workOrderClose-componentCollection`](#workorderclose-componentcollection) |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `createdFrom` |  | workOrder |  |  | [`workOrder`](workOrder.md#workorder) |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReason` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReasonMemo` | Deletion Reason Memo | string |  |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `excludeFromGLNumbering` | Exclude from GL Audit Numbering | boolean |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `item` |  | assemblyItem |  |  | [`assemblyItem`](assemblyItem.md#assemblyitem) |  |
| `lastModifiedDate` | Date Last Modified | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `manufacturingRouting` | Manufacturing Routing | integer | int64 |  |  |  |
| `memo` | Memo | string |  |  |  |  |
| `orderQuantity` | Work Order Quantity | number | float |  |  |  |
| `postingPeriod` |  | accountingPeriod |  |  | [`accountingPeriod`](accountingPeriod.md#accountingperiod) |  |
| `prevDate` | Previous Effective Date | string | date |  |  |  |
| `quantity` | Quantity | number | float |  |  |  |
| `quantityVarianceAmount` | Quantity Variance Amount | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revision` |  | itemRevision |  |  | [`itemRevision`](itemRevision.md#itemrevision) |  |
| `revisionMemo` | Revision Memo | string |  |  |  |  |
| `routingItem` |  | workOrderClose-routingItemCollection |  |  | [`workOrderClose-routingItemCollection`](#workorderclose-routingitemcollection) |  |
| `scrapAmount` | Scrap Amount | number | double |  |  |  |
| `scrapQuantity` | Scrap Quantity | number | float |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `total` | Projected Value | number | double |  |  |  |
| `tranDate` | Date | string | date |  |  |  |
| `tranId` | Ref No. | string |  |  |  |  |
| `transactionNumber` | Transaction Number | string |  |  |  |  |

## workOrderClose-componentCollection

Browser definition `workOrderClose-componentCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | workOrderClose-componentElement[] |  |  | [`workOrderClose-componentElement`](#workorderclose-componentelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## workOrderClose-componentElement

Browser definition `workOrderClose-componentElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `compItemName` | Component | string |  |  |  |  |
| `isNonInventory` | Non-inventory Item | boolean |  |  |  |  |
| `item` | Item ID | string |  |  |  |  |
| `lineNumber` | Line Number | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `orderQuantity` | Work Order Quantity | number | float |  |  |  |
| `quantity` | Quantity Consumed | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `unitCost` | Unit Cost | number | float |  |  |  |

## workOrderClose-routingItemCollection

Browser definition `workOrderClose-routingItemCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | workOrderClose-routingItemElement[] |  |  | [`workOrderClose-routingItemElement`](#workorderclose-routingitemelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## workOrderClose-routingItemElement

Browser definition `workOrderClose-routingItemElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `assignmentId` |  | integer | int64 |  |  |  |
| `item` |  | string |  |  |  |  |
| `itemName` | Item | string |  |  |  |  |
| `lineId` |  | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `operationName` | Operation Name | string |  |  |  |  |
| `operationSequence` | Operation Sequence | integer | int64 |  |  |  |
| `orderDoc` |  | integer | int64 |  |  |  |
| `orderLine` |  | integer | int64 |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `totalCost` |  | number | float |  |  |  |
| `totalTime` | Total Time (Min) | number | float |  |  |  |
| `totalTimeHours` |  | number | float |  |  |  |
| `unitCost` |  | number | float |  |  |  |

## workOrderCloseCollection

Browser definition `workOrderCloseCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | workOrderClose[] |  |  | [`workOrderClose`](#workorderclose) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## workOrderCloseSelectOptions

Browser definition `workOrderCloseSelectOptions`.

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
| `postingPeriod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `revision` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
