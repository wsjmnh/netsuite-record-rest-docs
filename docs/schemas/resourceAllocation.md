# Schemas: resourceAllocation

Property tables for definitions owned by `resourceAllocation`.

Record page: [resourceAllocation](../records/resourceAllocation.md).

## Index

- [resourceAllocation](#resourceallocation) — 26 properties
- [resourceAllocationCollection](#resourceallocationcollection) — 6 properties
- [resourceAllocationSelectOptions](#resourceallocationselectoptions) — 9 properties

## resourceAllocation

Browser definition `resourceAllocation`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `allocationAmount` | Allocate | number | float |  |  |  |
| `allocationResource` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `allocationType` |  | object |  |  |  |  |
| `allocationType.id` | Internal identifier | string |  |  |  | `1`, `2` |
| `allocationType.refName` | Reference Name | string |  |  |  |  |
| `allocationUnit` |  | object |  |  |  |  |
| `allocationUnit.id` | Internal identifier | string |  |  |  | `H`, `P` |
| `allocationUnit.refName` | Reference Name | string |  |  |  |  |
| `approvalStatus` |  | object |  |  |  |  |
| `approvalStatus.id` | Internal identifier | string |  |  |  | `11`, `12`, `13`, `14`, `15`, `16`, `17`, `18`, `19`, `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`, `10` |
| `approvalStatus.refName` | Reference Name | string |  |  |  |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `endDate` | End Date | string | date |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `nextApprover` |  | employee |  |  | [`employee`](employee.md#employee) |  |
| `notes` | Notes | string |  |  |  |  |
| `numberHours` | Number of Hours | number | float |  |  |  |
| `percentOfTime` | Percentage of Time | number | float |  |  |  |
| `project` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `projectTask` |  | projectTask |  |  | [`projectTask`](projectTask.md#projecttask) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `requestedBy` |  | employee |  |  | [`employee`](employee.md#employee) |  |
| `startDate` | Start Date | string | date |  |  |  |

## resourceAllocationCollection

Browser definition `resourceAllocationCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | resourceAllocation[] |  |  | [`resourceAllocation`](#resourceallocation) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## resourceAllocationSelectOptions

Browser definition `resourceAllocationSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `allocationResource` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `allocationType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `allocationUnit` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `approvalStatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `nextApprover` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `project` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `projectTask` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `requestedBy` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
