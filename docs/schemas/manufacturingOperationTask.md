# Schemas: manufacturingOperationTask

Property tables for definitions owned by `manufacturingOperationTask`.

Record page: [manufacturingOperationTask](../records/manufacturingOperationTask.md).

## Index

- [manufacturingOperationTask](#manufacturingoperationtask) — 33 properties
- [manufacturingOperationTask-costDetailCollection](#manufacturingoperationtask-costdetailcollection) — 6 properties
- [manufacturingOperationTask-costDetailElement](#manufacturingoperationtask-costdetailelement) — 6 properties
- [manufacturingOperationTask-predecessorCollection](#manufacturingoperationtask-predecessorcollection) — 6 properties
- [manufacturingOperationTask-predecessorElement](#manufacturingoperationtask-predecessorelement) — 13 properties
- [manufacturingOperationTaskCollection](#manufacturingoperationtaskcollection) — 6 properties
- [manufacturingOperationTaskSelectOptions](#manufacturingoperationtaskselectoptions) — 6 properties

## manufacturingOperationTask

Browser definition `manufacturingOperationTask`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `actualRunTime` | Actual Run Time (Min) | number | float |  |  |  |
| `actualSetupTime` | Actual Setup Time (Min) | number | float |  |  |  |
| `actualWork` | Actual Work | string |  |  |  |  |
| `autoCalculateLag` | Auto-calculate Lag | boolean |  |  |  |  |
| `completedQuantity` | Completed Quantity | number | float |  |  |  |
| `costDetail` |  | manufacturingOperationTask-costDetailCollection |  |  | [`manufacturingOperationTask-costDetailCollection`](#manufacturingoperationtask-costdetailcollection) |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `endDate` | End Date | string | date-time |  |  |  |
| `estimatedWork` | Estimated Work | number | float |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `inputQuantity` | Input Quantity | number | float |  |  |  |
| `insertBefore` |  | manufacturingOperationTask |  |  | [`manufacturingOperationTask`](#manufacturingoperationtask) |  |
| `laborResources` | Labor Resources | number | float |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `machineResources` | Machine Resources | number | float |  |  |  |
| `manufacturingCostTemplate` |  | manufacturingCostTemplate |  |  | [`manufacturingCostTemplate`](manufacturingCostTemplate.md#manufacturingcosttemplate) |  |
| `manufacturingWorkCenter` |  | entityGroup |  |  | [`entityGroup`](entityGroup.md#entitygroup) |  |
| `message` | Comments | string |  |  |  |  |
| `operationSequence` | Operation Sequence | integer | int64 |  |  |  |
| `predecessor` |  | manufacturingOperationTask-predecessorCollection |  |  | [`manufacturingOperationTask-predecessorCollection`](#manufacturingoperationtask-predecessorcollection) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `remainingWork` | Remaining Work | string |  |  |  |  |
| `runRate` | Run Rate (Min/Unit) | number | float |  |  |  |
| `setupTime` | Setup Time (Min) | number | float |  |  |  |
| `startDateTime` | Start Date | string | date-time |  |  |  |
| `status` |  | object |  |  |  |  |
| `status.id` | Internal identifier | string |  |  |  | `NOTSTART`, `PROGRESS`, `COMPLETE` |
| `status.refName` | Reference Name | string |  |  |  |  |
| `title` | Name | string |  |  |  |  |
| `units` | Units of Measure | string |  |  |  |  |
| `workOrder` |  | workOrder |  |  | [`workOrder`](workOrder.md#workorder) |  |

## manufacturingOperationTask-costDetailCollection

Browser definition `manufacturingOperationTask-costDetailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | manufacturingOperationTask-costDetailElement[] |  |  | [`manufacturingOperationTask-costDetailElement`](#manufacturingoperationtask-costdetailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## manufacturingOperationTask-costDetailElement

Browser definition `manufacturingOperationTask-costDetailElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `costCategory` |  | costCategory |  |  | [`costCategory`](costCategory.md#costcategory) |  |
| `fixedRate` | Fixed Rate | number | double |  |  |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `runRate` | Run Rate | number | double |  |  |  |

## manufacturingOperationTask-predecessorCollection

Browser definition `manufacturingOperationTask-predecessorCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | manufacturingOperationTask-predecessorElement[] |  |  | [`manufacturingOperationTask-predecessorElement`](#manufacturingoperationtask-predecessorelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## manufacturingOperationTask-predecessorElement

Browser definition `manufacturingOperationTask-predecessorElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `endDate` | End Date | string | date-time |  |  |  |
| `lagAmount` | Lag Amount | integer | int64 |  |  |  |
| `lagType` |  | object |  |  |  |  |
| `lagType.id` | Internal identifier | string |  |  |  | `quantity`, `timepercent`, `time`, `qtypercent` |
| `lagType.refName` | Reference Name | string |  |  |  |  |
| `lagUnits` | Lag Units | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `startDate` | Start Date | string | date-time |  |  |  |
| `task` |  | manufacturingOperationTask |  |  | [`manufacturingOperationTask`](#manufacturingoperationtask) |  |
| `type` |  | object |  |  |  |  |
| `type.id` | Internal identifier | string |  |  |  | `FS`, `SS` |
| `type.refName` | Reference Name | string |  |  |  |  |

## manufacturingOperationTaskCollection

Browser definition `manufacturingOperationTaskCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | manufacturingOperationTask[] |  |  | [`manufacturingOperationTask`](#manufacturingoperationtask) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## manufacturingOperationTaskSelectOptions

Browser definition `manufacturingOperationTaskSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `insertBefore` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `manufacturingCostTemplate` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `manufacturingWorkCenter` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `status` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `workOrder` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
