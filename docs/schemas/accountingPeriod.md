# Schemas: accountingPeriod

Property tables for definitions owned by `accountingPeriod`.

Record page: [accountingPeriod](../records/accountingPeriod.md).

## Index

- [accountingPeriod](#accountingperiod) — 24 properties
- [accountingPeriod-fiscalCalendarsCollection](#accountingperiod-fiscalcalendarscollection) — 6 properties
- [accountingPeriod-fiscalCalendarsElement](#accountingperiod-fiscalcalendarselement) — 4 properties
- [accountingPeriod-perBookPeriodClosingCollection](#accountingperiod-perbookperiodclosingcollection) — 6 properties
- [accountingPeriod-perBookPeriodClosingElement](#accountingperiod-perbookperiodclosingelement) — 4 properties
- [accountingPeriodCollection](#accountingperiodcollection) — 6 properties
- [accountingPeriodSelectOptions](#accountingperiodselectoptions) — 2 properties

## accountingPeriod

Browser definition `accountingPeriod`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `allLocked` | All Locked | boolean |  |  |  |  |
| `allowNonGLChanges` | Allow Non-G/L Changes | boolean |  |  |  |  |
| `apLocked` | A/P Locked | boolean |  |  |  |  |
| `arLocked` | A/R Locked | boolean |  |  |  |  |
| `closed` | Closed | boolean |  |  |  |  |
| `closedOnDate` | Date Closed | string | date |  |  |  |
| `endDate` | End Date | string | date |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `fiscalCalendar` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `fiscalCalendars` |  | accountingPeriod-fiscalCalendarsCollection |  |  | [`accountingPeriod-fiscalCalendarsCollection`](#accountingperiod-fiscalcalendarscollection) |  |
| `id` | Internal ID | string |  |  |  |  |
| `isAdjust` | Period is Adjustment | boolean |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `isPosting` | Is Posting | boolean |  |  |  |  |
| `isQuarter` | Period is a Quarter | boolean |  |  |  |  |
| `isYear` | Period is a Year | boolean |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `parent` |  | accountingPeriod |  |  | [`accountingPeriod`](#accountingperiod) |  |
| `payrollLocked` | Payroll Locked | boolean |  |  |  |  |
| `perBookPeriodClosing` |  | accountingPeriod-perBookPeriodClosingCollection |  |  | [`accountingPeriod-perBookPeriodClosingCollection`](#accountingperiod-perbookperiodclosingcollection) |  |
| `periodName` | Period Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `startDate` | Start Date | string | date |  |  |  |

## accountingPeriod-fiscalCalendarsCollection

Browser definition `accountingPeriod-fiscalCalendarsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | accountingPeriod-fiscalCalendarsElement[] |  |  | [`accountingPeriod-fiscalCalendarsElement`](#accountingperiod-fiscalcalendarselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## accountingPeriod-fiscalCalendarsElement

Browser definition `accountingPeriod-fiscalCalendarsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `fiscalCalendar` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `parent` |  | accountingPeriod |  |  | [`accountingPeriod`](#accountingperiod) |  |
| `refName` | Reference Name | string |  |  |  |  |

## accountingPeriod-perBookPeriodClosingCollection

Browser definition `accountingPeriod-perBookPeriodClosingCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | accountingPeriod-perBookPeriodClosingElement[] |  |  | [`accountingPeriod-perBookPeriodClosingElement`](#accountingperiod-perbookperiodclosingelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## accountingPeriod-perBookPeriodClosingElement

Browser definition `accountingPeriod-perBookPeriodClosingElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | accountingBook |  |  | [`accountingBook`](accountingBook.md#accountingbook) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `periodClosed` | Closed | boolean |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## accountingPeriodCollection

Browser definition `accountingPeriodCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | accountingPeriod[] |  |  | [`accountingPeriod`](#accountingperiod) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## accountingPeriodSelectOptions

Browser definition `accountingPeriodSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `fiscalCalendar` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `parent` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
