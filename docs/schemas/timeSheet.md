# Schemas: timeSheet

Property tables for definitions owned by `timeSheet`.

Record page: [timeSheet](../records/timeSheet.md).

## Index

- [timeSheet](#timesheet) — 24 properties
- [timeSheetCollection](#timesheetcollection) — 6 properties
- [timeSheetSelectOptions](#timesheetselectoptions) — 5 properties

## timeSheet

Browser definition `timeSheet`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `allocatedhours` | Allocated Hours | string |  |  |  |  |
| `approvalStatus` |  | object |  |  |  |  |
| `approvalStatus.id` | Internal identifier | string |  |  |  | `1`, `2`, `3`, `4` |
| `approvalStatus.refName` | Reference Name | string |  |  |  |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `employee` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `endDate` | End Date | string | date |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `lockstatus` |  | object |  |  |  |  |
| `lockstatus.id` | Internal identifier | string |  |  |  | `unlocked`, `locked`, `partially` |
| `lockstatus.refName` | Reference Name | string |  |  |  |  |
| `name` | Name | string |  |  |  |  |
| `plannedhours` | Planned Hours | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `rejectedhours` | Rejected Hours | string |  |  |  |  |
| `startDate` | Start Date | string | date |  |  |  |
| `submittedhours` | Submitted hours | string |  |  |  |  |
| `subsidiary` | Subsidiary | string |  |  |  |  |
| `totalHours` | Total Hours | string |  |  |  |  |
| `tranDate` | Week Of | string | date |  |  |  |
| `workcalendarhours` | Work Calendar Hours | string |  |  |  |  |

## timeSheetCollection

Browser definition `timeSheetCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | timeSheet[] |  |  | [`timeSheet`](#timesheet) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## timeSheetSelectOptions

Browser definition `timeSheetSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `approvalStatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `employee` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `lockstatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
