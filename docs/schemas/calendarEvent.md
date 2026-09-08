# Schemas: calendarEvent

Property tables for definitions owned by `calendarEvent`.

Record page: [calendarEvent](../records/calendarEvent.md).

## Index

- [calendarEvent](#calendarevent) — 46 properties
- [calendarEvent-attendeeCollection](#calendarevent-attendeecollection) — 6 properties
- [calendarEvent-attendeeElement](#calendarevent-attendeeelement) — 9 properties
- [calendarEvent-resourceCollection](#calendarevent-resourcecollection) — 6 properties
- [calendarEvent-resourceElement](#calendarevent-resourceelement) — 3 properties
- [calendarEvent-timeItemCollection](#calendarevent-timeitemcollection) — 6 properties
- [calendarEvent-timeItemElement](#calendarevent-timeitemelement) — 24 properties
- [calendarEventCollection](#calendareventcollection) — 6 properties
- [calendarEventSelectOptions](#calendareventselectoptions) — 16 properties

## calendarEvent

Browser definition `calendarEvent`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accessLevel` |  | object |  |  |  |  |
| `accessLevel.id` | Internal identifier | string |  |  |  | `PUBLIC`, `PRIVATE`, `SHOW AS BUSY` |
| `accessLevel.refName` | Reference Name | string |  |  |  |  |
| `allDayEvent` | All Day | boolean |  |  |  |  |
| `attendee` |  | calendarEvent-attendeeCollection |  |  | [`calendarEvent-attendeeCollection`](#calendarevent-attendeecollection) |  |
| `bom` |  | bom |  |  | [`bom`](bom.md#bom) |  |
| `bomRevision` |  | bomRevision |  |  | [`bomRevision`](bomRevision.md#bomrevision) |  |
| `company` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `completedDate` | Completed Date | string | date |  |  |  |
| `contact` |  | contact |  |  | [`contact`](contact.md#contact) |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `endTime` | End time | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` | Location | string |  |  |  |  |
| `message` | Message | string |  |  |  |  |
| `mfgRouting` |  | manufacturingRouting |  |  | [`manufacturingRouting`](manufacturingRouting.md#manufacturingrouting) |  |
| `organizer` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `owner` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `recurrence` | Recurrence | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `relatedItem` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `reminderMinutes` |  | object |  |  |  |  |
| `reminderMinutes.id` | Internal identifier | string |  |  |  | `0`, `5`, `10`, `15`, `30` |
| `reminderMinutes.refName` | Reference Name | string |  |  |  |  |
| `reminderType` |  | object |  |  |  |  |
| `reminderType.id` | Internal identifier | string |  |  |  | `POPUP`, `EMAIL` |
| `reminderType.refName` | Reference Name | string |  |  |  |  |
| `resource` |  | calendarEvent-resourceCollection |  |  | [`calendarEvent-resourceCollection`](#calendarevent-resourcecollection) |  |
| `response` |  | object |  |  |  |  |
| `response.id` | Internal identifier | string |  |  |  | `TENTATIVE`, `ACCEPTED`, `ESCALATED`, `NO_RESPONSE`, `DECLINED` |
| `response.refName` | Reference Name | string |  |  |  |  |
| `startDate` | Start Date | string | date |  |  |  |
| `startTime` | Start Time | string |  |  |  |  |
| `status` |  | object |  |  |  |  |
| `status.id` | Internal identifier | string |  |  |  | `TENTATIVE`, `CONFIRMED`, `COMPLETE`, `CANCELLED` |
| `status.refName` | Reference Name | string |  |  |  |  |
| `supportCase` |  | supportCase |  |  | [`supportCase`](supportCase.md#supportcase) |  |
| `timeItem` |  | calendarEvent-timeItemCollection |  |  | [`calendarEvent-timeItemCollection`](#calendarevent-timeitemcollection) |  |
| `timedEvent` | Timed Event | boolean |  |  |  |  |
| `timezone` | Time Zone | string |  |  |  |  |
| `title` | Title | string |  |  |  |  |
| `transaction` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |

## calendarEvent-attendeeCollection

Browser definition `calendarEvent-attendeeCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | calendarEvent-attendeeElement[] |  |  | [`calendarEvent-attendeeElement`](#calendarevent-attendeeelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## calendarEvent-attendeeElement

Browser definition `calendarEvent-attendeeElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `attendance` |  | object |  |  |  |  |
| `attendance.id` | Internal identifier | string |  |  |  | `REQUIRED`, `OPTIONAL` |
| `attendance.refName` | Reference Name | string |  |  |  |  |
| `attendee` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `response` |  | object |  |  |  |  |
| `response.id` | Internal identifier | string |  |  |  | `ACCEPTED`, `DECLINED`, `TENTATIVE`, `NO_RESPONSE` |
| `response.refName` | Reference Name | string |  |  |  |  |

## calendarEvent-resourceCollection

Browser definition `calendarEvent-resourceCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | calendarEvent-resourceElement[] |  |  | [`calendarEvent-resourceElement`](#calendarevent-resourceelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## calendarEvent-resourceElement

Browser definition `calendarEvent-resourceElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `resource` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |

## calendarEvent-timeItemCollection

Browser definition `calendarEvent-timeItemCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | calendarEvent-timeItemElement[] |  |  | [`calendarEvent-timeItemElement`](#calendarevent-timeitemelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## calendarEvent-timeItemElement

Browser definition `calendarEvent-timeItemElement`.

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

## calendarEventCollection

Browser definition `calendarEventCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | calendarEvent[] |  |  | [`calendarEvent`](#calendarevent) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## calendarEventSelectOptions

Browser definition `calendarEventSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accessLevel` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `bom` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `bomRevision` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `company` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `contact` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `mfgRouting` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `organizer` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `owner` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `relatedItem` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `reminderMinutes` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `reminderType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `response` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `status` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `supportCase` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `transaction` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
