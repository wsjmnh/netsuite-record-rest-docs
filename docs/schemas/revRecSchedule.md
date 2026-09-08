# Schemas: revRecSchedule

Property tables for definitions owned by `revRecSchedule`.

Record page: [revRecSchedule](../records/revRecSchedule.md).

## Index

- [revRecSchedule](#revrecschedule) — 46 properties
- [revRecSchedule-recurrenceCollection](#revrecschedule-recurrencecollection) — 6 properties
- [revRecSchedule-recurrenceElement](#revrecschedule-recurrenceelement) — 16 properties
- [revRecScheduleCollection](#revrecschedulecollection) — 6 properties
- [revRecScheduleSelectOptions](#revrecscheduleselectoptions) — 9 properties

## revRecSchedule

Browser definition `revRecSchedule`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | accountingBook |  |  | [`accountingBook`](accountingBook.md#accountingbook) |  |
| `amortizationPeriod` | Recognition Period | integer | int64 |  |  |  |
| `amortizationType` |  | object |  |  |  |  |
| `amortizationType.id` | Internal identifier | string |  |  |  | `STANDARD`, `VARIABLE` |
| `amortizationType.refName` | Reference Name | string |  |  |  |  |
| `baseCurrencyPrecision` | Base Currency Precision | integer | int64 |  |  |  |
| `endDate` | End Date | string | date |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `forecastTemplate` |  | revRecTemplate |  |  | [`revRecTemplate`](revRecTemplate.md#revrectemplate) |  |
| `id` | Internal ID | string |  |  |  |  |
| `initialAmount` | Initial Amount | number | double |  |  |  |
| `isAmortization` | Is Amortization | boolean |  |  |  |  |
| `isEliminate` | Eliminate | boolean |  |  |  |  |
| `isEstimate` | Estimate | boolean |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `isRecognized` | Is Recognized | boolean |  |  |  |  |
| `isSchedule` | Is Schedule | boolean |  |  |  |  |
| `job` |  | job |  |  | [`job`](job.md#job) |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Name | string |  |  |  |  |
| `parentSched` |  | revRecTemplate |  |  | [`revRecTemplate`](revRecTemplate.md#revrectemplate) |  |
| `periodOffset` | Period Offset | integer | int64 |  |  |  |
| `recogIntervalSrc` |  | object |  |  |  |  |
| `recogIntervalSrc.id` | Internal identifier | string |  |  |  | `RECEIPTDATE`, `USERDEFINED`, `BETWEENBILLS`, `BETWEENBILLSRRDATE`, `SOREVRECDATES` |
| `recogIntervalSrc.refName` | Reference Name | string |  |  |  |  |
| `recurrence` |  | revRecSchedule-recurrenceCollection |  |  | [`revRecSchedule-recurrenceCollection`](#revrecschedule-recurrencecollection) |  |
| `recurrenceType` |  | object |  |  |  |  |
| `recurrenceType.id` | Internal identifier | string |  |  |  | `DATESPRORATE`, `EVENPERIODSPRORATE`, `CUSTOM`, `EVENPRORATEPERIOD`, `DATESINTOPERIODS` |
| `recurrenceType.refName` | Reference Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `remainingDeferredBalance` | Remaining Deferred Balance | number | double |  |  |  |
| `revRecNumber` | Rev Rec Number | string |  |  |  |  |
| `revRecOffset` | Start Offset | integer | int64 |  |  |  |
| `scheduleNumber` | Number | string |  |  |  |  |
| `sourceTran` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `startDate` | Start Date | string | date |  |  |  |
| `status` |  | object |  |  |  |  |
| `status.id` | Internal identifier | string |  |  |  | `NOTSTARTED`, `INPROGRESS`, `COMPLETED`, `ONHOLD` |
| `status.refName` | Reference Name | string |  |  |  |  |
| `subsidiary` | Subsidiary | string |  |  |  |  |
| `target` | Target | string |  |  |  |  |
| `totalAmortized` | Total Recognized | number | double |  |  |  |
| `totalAmount` | Amount (Schedule Total) | number | double |  |  |  |
| `tranLineId` | Source Transaction Line | string |  |  |  |  |
| `tranType` | Tran Type | string |  |  |  |  |

## revRecSchedule-recurrenceCollection

Browser definition `revRecSchedule-recurrenceCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | revRecSchedule-recurrenceElement[] |  |  | [`revRecSchedule-recurrenceElement`](#revrecschedule-recurrenceelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## revRecSchedule-recurrenceElement

Browser definition `revRecSchedule-recurrenceElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `defRevAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `id` |  | integer | int64 |  |  |  |
| `incomeAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `isRecognized` | Is Recognized | boolean |  |  |  |  |
| `jDate` | Date Executed | string | date |  |  |  |
| `journal` | Journal | string |  |  |  |  |
| `journalDoc` | Journal ID | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `pctAmortInPeriod` | % Amortized In Period | number | double |  |  |  |
| `pctTotalAmortization` | % Total Amortized | number | double |  |  |  |
| `periodOffset` | Period Offset | integer | int64 |  |  |  |
| `postingPeriod` |  | accountingPeriod |  |  | [`accountingPeriod`](accountingPeriod.md#accountingperiod) |  |
| `recAmount` | Amount | number | double |  |  |  |
| `recurDate` | Date | string | date |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `totalAmortizedMach` | Total Recognized | number | double |  |  |  |

## revRecScheduleCollection

Browser definition `revRecScheduleCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | revRecSchedule[] |  |  | [`revRecSchedule`](#revrecschedule) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## revRecScheduleSelectOptions

Browser definition `revRecScheduleSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `amortizationType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `forecastTemplate` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `job` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `parentSched` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `recogIntervalSrc` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `recurrenceType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `sourceTran` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `status` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
