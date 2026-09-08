# Schemas: phoneCall

Property tables for definitions owned by `phoneCall`.

Record page: [phoneCall](../records/phoneCall.md).

## Index

- [phoneCall](#phonecall) — 41 properties
- [phoneCall-timeItemCollection](#phonecall-timeitemcollection) — 6 properties
- [phoneCall-timeItemElement](#phonecall-timeitemelement) — 24 properties
- [phoneCallCollection](#phonecallcollection) — 6 properties
- [phoneCallSelectOptions](#phonecallselectoptions) — 15 properties

## phoneCall

Browser definition `phoneCall`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accessLevel` | Private | boolean |  |  |  |  |
| `assigned` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `bom` |  | bom |  |  | [`bom`](bom.md#bom) |  |
| `bomRevision` |  | bomRevision |  |  | [`bomRevision`](bomRevision.md#bomrevision) |  |
| `company` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `completedDate` | Date Completed | string | date |  |  |  |
| `contact` |  | contact |  |  | [`contact`](contact.md#contact) |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `endTime` | End time | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `message` | Comments | string |  |  |  |  |
| `mfgRouting` |  | manufacturingRouting |  |  | [`manufacturingRouting`](manufacturingRouting.md#manufacturingrouting) |  |
| `owner` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `phone` | Phone | string |  |  |  |  |
| `priority` |  | object |  |  |  |  |
| `priority.id` | Internal identifier | string |  |  |  | `HIGH`, `MEDIUM`, `LOW` |
| `priority.refName` | Reference Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `relatedItem` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `reminderMinutes` |  | object |  |  |  |  |
| `reminderMinutes.id` | Internal identifier | string |  |  |  | `0`, `5`, `10`, `15`, `30` |
| `reminderMinutes.refName` | Reference Name | string |  |  |  |  |
| `reminderType` |  | object |  |  |  |  |
| `reminderType.id` | Internal identifier | string |  |  |  | `POPUP`, `EMAIL` |
| `reminderType.refName` | Reference Name | string |  |  |  |  |
| `sendEmail` | Send email | boolean |  |  |  |  |
| `startDate` | Start Date | string | date |  |  |  |
| `startTime` | Start Time | string |  |  |  |  |
| `status` |  | object |  |  |  |  |
| `status.id` | Internal identifier | string |  |  |  | `SCHEDULED`, `FAILED`, `COMPLETE` |
| `status.refName` | Reference Name | string |  |  |  |  |
| `supportCase` |  | supportCase |  |  | [`supportCase`](supportCase.md#supportcase) |  |
| `timeItem` |  | phoneCall-timeItemCollection |  |  | [`phoneCall-timeItemCollection`](#phonecall-timeitemcollection) |  |
| `timedEvent` | Timed Event | boolean |  |  |  |  |
| `timezone` | Time Zone | string |  |  |  |  |
| `title` | Title | string |  |  |  |  |
| `transaction` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |

## phoneCall-timeItemCollection

Browser definition `phoneCall-timeItemCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | phoneCall-timeItemElement[] |  |  | [`phoneCall-timeItemElement`](#phonecall-timeitemelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## phoneCall-timeItemElement

Browser definition `phoneCall-timeItemElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `customer` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `employee` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `externalId` | External ID | string |  |  |  |  |
| `hours` | Duration | string |  |  |  |  |
| `id` | Internal ID | integer | int64 |  |  |  |
| `isBillable` | Billable | boolean |  |  |  |  |
| `isExempt` | Exempt | boolean |  |  |  |  |
| `isProductive` | Productive | boolean |  |  |  |  |
| `isUtilized` | Utilized | boolean |  |  |  |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `overrideRate` | Lock this Rate | boolean |  |  |  |  |
| `payrollItem` |  | payrollItem |  |  | [`payrollItem`](payrollItem.md#payrollitem) |  |
| `price` |  | priceLevel |  |  | [`priceLevel`](priceLevel.md#pricelevel) |  |
| `rate` | Rate | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `timeType` |  | object |  |  |  |  |
| `timeType.id` | Internal identifier | string |  |  |  | `P`, `A`, `B` |
| `timeType.refName` | Reference Name | string |  |  |  |  |
| `tranDate` | Date | string | date |  |  |  |

## phoneCallCollection

Browser definition `phoneCallCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | phoneCall[] |  |  | [`phoneCall`](#phonecall) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## phoneCallSelectOptions

Browser definition `phoneCallSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `assigned` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `bom` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `bomRevision` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `company` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `contact` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `mfgRouting` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `owner` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `priority` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `relatedItem` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `reminderMinutes` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `reminderType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `status` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `supportCase` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `transaction` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
