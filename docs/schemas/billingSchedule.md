# Schemas: billingSchedule

Property tables for definitions owned by `billingSchedule`.

Record page: [billingSchedule](../records/billingSchedule.md).

## Index

- [billingSchedule](#billingschedule) — 62 properties
- [billingSchedule-milestoneCollection](#billingschedule-milestonecollection) — 6 properties
- [billingSchedule-milestoneElement](#billingschedule-milestoneelement) — 10 properties
- [billingSchedule-recurrenceCollection](#billingschedule-recurrencecollection) — 6 properties
- [billingSchedule-recurrenceElement](#billingschedule-recurrenceelement) — 11 properties
- [billingScheduleCollection](#billingschedulecollection) — 6 properties
- [billingScheduleSelectOptions](#billingscheduleselectoptions) — 14 properties

## billingSchedule

Browser definition `billingSchedule`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `applyToSubtotal` | Apply To Subtotal | boolean |  |  |  |  |
| `billForActuals` | Invoice Actual Time Only | boolean |  |  |  |  |
| `dayPeriod` | Recurrence | integer | int64 |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `frequency` |  | object |  |  |  |  |
| `frequency.id` | Internal identifier | string |  |  |  | `SEMIMONTHLY`, `STARTOFPERIOD`, `WEEKLY`, `QUADWEEKLY`, `BIENNIALLY`, `DAILY`, `NEVER`, `ONETIME`, `SEMIANNUALLY`, `ENDOFPERIOD`, `MONTHLY`, `AUTOREFILL`, `TRIENNIALLY`, `HOURLY`, `QUARTERLY`, `ANNUALLY`, `CUSTOM`, `BIMONTHLY`, `BIWEEKLY` |
| `frequency.refName` | Reference Name | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `inArrears` | In Arrears | boolean |  |  |  |  |
| `initialAmount` | Initial Amount | number | double |  |  |  |
| `initialAmountPercent` | Initial Amount in % | number | double |  |  |  |
| `initialTerms` |  | term |  |  | [`term`](term.md#term) |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `isPublic` | Public | boolean |  |  |  |  |
| `job` |  | job |  |  | [`job`](job.md#job) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `milestone` |  | billingSchedule-milestoneCollection |  |  | [`billingSchedule-milestoneCollection`](#billingschedule-milestonecollection) |  |
| `monthDom` | Day of Month | integer | int64 |  |  |  |
| `monthDow` |  | object |  |  |  |  |
| `monthDow.id` | Internal identifier | string |  |  |  | `1`, `2`, `3`, `4`, `5`, `6`, `7`, `-1` |
| `monthDow.refName` | Reference Name | string |  |  |  |  |
| `monthDowim` |  | object |  |  |  |  |
| `monthDowim.id` | Internal identifier | string |  |  |  | `1`, `2`, `3`, `4`, `5` |
| `monthDowim.refName` | Reference Name | string |  |  |  |  |
| `monthMode` | Mode | string |  |  |  |  |
| `name` | Name | string |  |  |  |  |
| `numberRemaining` | Recurrence Count | integer | int64 |  |  |  |
| `recurrence` |  | billingSchedule-recurrenceCollection |  |  | [`billingSchedule-recurrenceCollection`](#billingschedule-recurrencecollection) |  |
| `recurrencePattern` |  | object |  |  |  |  |
| `recurrencePattern.id` | Internal identifier | string |  |  |  | `FIXED_BILL_DATE`, `ANNIVERSARY_BILL_DATE` |
| `recurrencePattern.refName` | Reference Name | string |  |  |  |  |
| `recurrenceTerms` |  | term |  |  | [`term`](term.md#term) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `repeatEvery` |  | object |  |  |  |  |
| `repeatEvery.id` | Internal identifier | string |  |  |  | `1`, `2`, `3`, `4`, `6` |
| `repeatEvery.refName` | Reference Name | string |  |  |  |  |
| `scheduleType` |  | object |  |  |  |  |
| `scheduleType.id` | Internal identifier | string |  |  |  | `1`, `2`, `3`, `4`, `5` |
| `scheduleType.refName` | Reference Name | string |  |  |  |  |
| `seriesStartDate` | Recurrence Date | string | date |  |  |  |
| `transaction` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `weekFriday` | Friday | boolean |  |  |  |  |
| `weekMonday` | Monday | boolean |  |  |  |  |
| `weekSaturday` | Saturday | boolean |  |  |  |  |
| `weekSunday` | Sunday | boolean |  |  |  |  |
| `weekThursday` | Thursday | boolean |  |  |  |  |
| `weekTuesday` | Tuesday | boolean |  |  |  |  |
| `weekWednesday` | Wednesday | boolean |  |  |  |  |
| `yearDom` | Day of Month | integer | int64 |  |  |  |
| `yearDow` |  | object |  |  |  |  |
| `yearDow.id` | Internal identifier | string |  |  |  | `1`, `2`, `3`, `4`, `5`, `6`, `7`, `-1` |
| `yearDow.refName` | Reference Name | string |  |  |  |  |
| `yearDowim` |  | object |  |  |  |  |
| `yearDowim.id` | Internal identifier | string |  |  |  | `1`, `2`, `3`, `4`, `5` |
| `yearDowim.refName` | Reference Name | string |  |  |  |  |
| `yearDowimMonth` |  | object |  |  |  |  |
| `yearDowimMonth.id` | Internal identifier | string |  |  |  | `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`, `10`, `11`, `12` |
| `yearDowimMonth.refName` | Reference Name | string |  |  |  |  |
| `yearMode` | Mode | string |  |  |  |  |
| `yearMonth` |  | object |  |  |  |  |
| `yearMonth.id` | Internal identifier | string |  |  |  | `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`, `10`, `11`, `12` |
| `yearMonth.refName` | Reference Name | string |  |  |  |  |

## billingSchedule-milestoneCollection

Browser definition `billingSchedule-milestoneCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | billingSchedule-milestoneElement[] |  |  | [`billingSchedule-milestoneElement`](#billingschedule-milestoneelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## billingSchedule-milestoneElement

Browser definition `billingSchedule-milestoneElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `comments` | Comment | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `milestoneActualCompletionDate` | Actual Completion Date | string | date |  |  |  |
| `milestoneAmount` | Amount | number | double |  |  |  |
| `milestoneCompleted` | Completed | boolean |  |  |  |  |
| `milestoneDate` | Estimated Completion Date | string | date |  |  |  |
| `milestoneId` |  | number | double |  |  |  |
| `milestoneTerms` |  | term |  |  | [`term`](term.md#term) |  |
| `projectTask` |  | projectTask |  |  | [`projectTask`](projectTask.md#projecttask) |  |
| `refName` | Reference Name | string |  |  |  |  |

## billingSchedule-recurrenceCollection

Browser definition `billingSchedule-recurrenceCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | billingSchedule-recurrenceElement[] |  |  | [`billingSchedule-recurrenceElement`](#billingschedule-recurrenceelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## billingSchedule-recurrenceElement

Browser definition `billingSchedule-recurrenceElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amount` | Amount | number | double |  |  |  |
| `count` | Count | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `paymentTerms` |  | term |  |  | [`term`](term.md#term) |  |
| `recurrenceDate` | Date | string | date |  |  |  |
| `recurrenceId` |  | integer | int64 |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `relativeToPrevious` | Relative to Previous | boolean |  |  |  |  |
| `units` |  | object |  |  |  |  |
| `units.id` | Internal identifier | string |  |  |  | `DAY`, `WEEK`, `MONTH` |
| `units.refName` | Reference Name | string |  |  |  |  |

## billingScheduleCollection

Browser definition `billingScheduleCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | billingSchedule[] |  |  | [`billingSchedule`](#billingschedule) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## billingScheduleSelectOptions

Browser definition `billingScheduleSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `frequency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `initialTerms` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `job` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `monthDow` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `monthDowim` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `recurrencePattern` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `recurrenceTerms` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `repeatEvery` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `scheduleType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `transaction` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `yearDow` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `yearDowim` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `yearDowimMonth` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `yearMonth` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
