# Schemas: timeBill

Property tables for definitions owned by `timeBill`.

Record page: [timeBill](../records/timeBill.md).

## Index

- [timeBill](#timebill) — 45 properties
- [timeBillCollection](#timebillcollection) — 6 properties
- [timeBillSelectOptions](#timebillselectoptions) — 20 properties

## timeBill

Browser definition `timeBill`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `approvalStatus` |  | object |  |  |  |  |
| `approvalStatus.id` | Internal identifier | string |  |  |  | `1`, `2`, `3`, `4` |
| `approvalStatus.refName` | Reference Name | string |  |  |  |  |
| `billingClass` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `billingSubsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `caseTaskEvent` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `customer` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `displayField` | Time Tracking | string |  |  |  |  |
| `employee` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `externalId` | External ID | string |  |  |  |  |
| `hours` | Duration | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isBillable` | Billable | boolean |  |  |  |  |
| `isExempt` | Exempt | boolean |  |  |  |  |
| `isProductive` | Productive | boolean |  |  |  |  |
| `isUtilized` | Utilized | boolean |  |  |  |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `nextApprover` |  | employee |  |  | [`employee`](employee.md#employee) |  |
| `overrideRate` | Lock this Rate | boolean |  |  |  |  |
| `paidExternally` | Paid Externally | boolean |  |  |  |  |
| `payrollItem` |  | payrollItem |  |  | [`payrollItem`](payrollItem.md#payrollitem) |  |
| `payrollWorkplace` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `posted` | Posted | boolean |  |  |  |  |
| `price` |  | priceLevel |  |  | [`priceLevel`](priceLevel.md#pricelevel) |  |
| `rate` | Rate | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `rejectionNote` | Rejection Note | string |  |  |  |  |
| `resourceAllocation` |  | resourceAllocation |  |  | [`resourceAllocation`](resourceAllocation.md#resourceallocation) |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `supervisorApproval` | Supervisor Approval | boolean |  |  |  |  |
| `timeModified` | Time Modified | boolean |  |  |  |  |
| `timeOffType` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `timeType` |  | object |  |  |  |  |
| `timeType.id` | Internal identifier | string |  |  |  | `P`, `A`, `B` |
| `timeType.refName` | Reference Name | string |  |  |  |  |
| `timesheet` |  | timeSheet |  |  | [`timeSheet`](timeSheet.md#timesheet) |  |
| `tranDate` | Date | string | date |  |  |  |

## timeBillCollection

Browser definition `timeBillCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | timeBill[] |  |  | [`timeBill`](#timebill) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## timeBillSelectOptions

Browser definition `timeBillSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `approvalStatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billingClass` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billingSubsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `caseTaskEvent` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customer` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `employee` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `item` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `nextApprover` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `payrollItem` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `payrollWorkplace` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `price` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `resourceAllocation` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `timeOffType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `timeType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `timesheet` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
