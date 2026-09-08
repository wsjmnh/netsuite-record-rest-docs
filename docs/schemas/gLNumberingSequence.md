# Schemas: gLNumberingSequence

Property tables for definitions owned by `gLNumberingSequence`.

Record page: [gLNumberingSequence](../records/gLNumberingSequence.md).

## Index

- [gLNumberingSequence](#glnumberingsequence) — 37 properties
- [gLNumberingSequenceCollection](#glnumberingsequencecollection) — 6 properties
- [gLNumberingSequenceSelectOptions](#glnumberingsequenceselectoptions) — 10 properties

## gLNumberingSequence

Browser definition `gLNumberingSequence`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | accountingBook |  |  | [`accountingBook`](accountingBook.md#accountingbook) |  |
| `dailyRecurring` |  | object |  |  |  |  |
| `dailyRecurring.id` | Internal identifier | string |  |  |  | `EVERYDAY`, `MONDAY`, `TUESDAY`, `WEDNESDAY`, `THURSDAY`, `FRIDAY`, `SATURDAY`, `SUNDAY` |
| `dailyRecurring.refName` | Reference Name | string |  |  |  |  |
| `excludeZeroTransactions` | Exclude zero amount transactions | boolean |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `firstRun` |  | object |  |  |  |  |
| `firstRun.id` | Internal identifier | string |  |  |  | `1000`, `2330`, `2230`, `2130`, `2030`, `130`, `230`, `330`, `430`, `530`, `1930`, `630`, `1830`, `730`, `1730`, `830`, `1630`, `930`, `1530`, `2300`, `1430`, `2200`, `30`, `1330`, `2100`, `1230`, `2000`, `1130`, `1030`, `0`, `1800`, `100`, `1700`, `200`, `1600`, `300`, `1500`, `400`, `1400`, `500`, `1300`, `600`, `1200`, `700`, `1100`, `800`, `900`, `1900` |
| `firstRun.refName` | Reference Name | string |  |  |  |  |
| `hourlyRecurring` | Hourly Recurring | integer | int64 |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `initNum` | Initial Number | integer | int64 |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `lastAssigned` | Last Assigned | integer | int64 |  |  |  |
| `lastRunBy` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `lastRunDate` | Last Run | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `minDigits` | Minimum Digits | integer | int64 |  |  |  |
| `nextRun` | Next Run | string | date-time |  |  |  |
| `numberingType` |  | object |  |  |  |  |
| `numberingType.id` | Internal identifier | string |  |  |  | `REPEATABLE`, `PERMANENT` |
| `numberingType.refName` | Reference Name | string |  |  |  |  |
| `orderType` |  | object |  |  |  |  |
| `orderType.id` | Internal identifier | string |  |  |  | `CREATEDDATE`, `TRANDATE` |
| `orderType.refName` | Reference Name | string |  |  |  |  |
| `period` |  | accountingPeriod |  |  | [`accountingPeriod`](accountingPeriod.md#accountingperiod) |  |
| `prefix` | Prefix | string |  |  |  |  |
| `recurringType` |  | object |  |  |  |  |
| `recurringType.id` | Internal identifier | string |  |  |  | `NONE`, `HOURLY`, `DAILY` |
| `recurringType.refName` | Reference Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `sequenceName` | Name | string |  |  |  |  |
| `status` |  | object |  |  |  |  |
| `status.id` | Internal identifier | string |  |  |  | `VALID`, `INVALID`, `RUNNING` |
| `status.refName` | Reference Name | string |  |  |  |  |
| `subsidiaries` |  | subsidiaryCollection |  |  | [`subsidiaryCollection`](subsidiary.md#subsidiarycollection) |  |
| `suffix` | Suffix | string |  |  |  |  |

## gLNumberingSequenceCollection

Browser definition `gLNumberingSequenceCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | gLNumberingSequence[] |  |  | [`gLNumberingSequence`](#glnumberingsequence) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## gLNumberingSequenceSelectOptions

Browser definition `gLNumberingSequenceSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `dailyRecurring` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `firstRun` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `lastRunBy` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `numberingType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `orderType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `period` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `recurringType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `status` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiaries` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
