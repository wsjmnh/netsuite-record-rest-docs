# Schemas: term

Property tables for definitions owned by `term`.

Record page: [term](../records/term.md).

## Index

- [term](#term) — 29 properties
- [term-percentagesCollection](#term-percentagescollection) — 6 properties
- [term-percentagesElement](#term-percentageselement) — 4 properties
- [termCollection](#termcollection) — 6 properties
- [termSelectOptions](#termselectoptions) — 2 properties

## term

Browser definition `term`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `dateDriven` |  | object |  |  |  |  |
| `dateDriven.id` | Internal identifier | string |  |  |  |  |
| `dateDriven.refName` | Reference Name | string |  |  |  |  |
| `dayDiscountExpires` | Day Discount Expires | integer | int64 |  |  |  |
| `dayOfMonthNetDue` | Day Of Month Net Due | integer | int64 |  |  |  |
| `daysUntilExpiry` | Days Till Discount Expires | integer | int64 |  |  |  |
| `daysUntilNetDue` | Days Till Net Due | integer | int64 |  |  |  |
| `discountPercent` | % Discount | number | float |  |  |  |
| `discountPercentDateDriven` | Date Driven % Discount | number | float |  |  |  |
| `dueNextMonthIfWithinDays` | Due Next Month If Within Days | integer | int64 |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `installment` | Installment | boolean |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `longitemtype` |  | string |  |  |  |  |
| `name` | Terms | string |  |  |  |  |
| `payTaxUpfront` | Pay Tax Upfront | boolean |  |  |  |  |
| `percentages` |  | term-percentagesCollection |  |  | [`term-percentagesCollection`](#term-percentagescollection) |  |
| `preferred` | Preferred | boolean |  |  |  |  |
| `recurrenceCount` | Recurrence Count | integer | int64 |  |  |  |
| `recurrenceFrequency` |  | object |  |  |  |  |
| `recurrenceFrequency.id` | Internal identifier | string |  |  |  | `SEMIMONTHLY`, `STARTOFPERIOD`, `WEEKLY`, `QUADWEEKLY`, `BIENNIALLY`, `DAILY`, `NEVER`, `ONETIME`, `SEMIANNUALLY`, `ENDOFPERIOD`, `MONTHLY`, `AUTOREFILL`, `TRIENNIALLY`, `HOURLY`, `QUARTERLY`, `ANNUALLY`, `CUSTOM`, `BIMONTHLY`, `BIWEEKLY` |
| `recurrenceFrequency.refName` | Reference Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `repeatEvery` | Repeat Every | integer | int64 |  |  |  |
| `splitEvenly` | Split Evenly | boolean |  |  |  |  |
| `tname` |  | string |  |  |  |  |

## term-percentagesCollection

Browser definition `term-percentagesCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | term-percentagesElement[] |  |  | [`term-percentagesElement`](#term-percentageselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## term-percentagesElement

Browser definition `term-percentagesElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `installmentLineNum` | # | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `percentage` | Percentage | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## termCollection

Browser definition `termCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | term[] |  |  | [`term`](#term) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## termSelectOptions

Browser definition `termSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `dateDriven` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `recurrenceFrequency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
