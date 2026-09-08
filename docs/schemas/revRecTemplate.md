# Schemas: revRecTemplate

Property tables for definitions owned by `revRecTemplate`.

Record page: [revRecTemplate](../records/revRecTemplate.md).

## Index

- [revRecTemplate](#revrectemplate) — 28 properties
- [revRecTemplate-recurrenceCollection](#revrectemplate-recurrencecollection) — 6 properties
- [revRecTemplate-recurrenceElement](#revrectemplate-recurrenceelement) — 7 properties
- [revRecTemplateCollection](#revrectemplatecollection) — 6 properties
- [revRecTemplateSelectOptions](#revrectemplateselectoptions) — 4 properties

## revRecTemplate

Browser definition `revRecTemplate`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amortizationPeriod` | Recognition Period | integer | int64 |  |  |  |
| `amortizationType` |  | object |  |  |  |  |
| `amortizationType.id` | Internal identifier | string |  |  |  | `STANDARD`, `VARIABLE` |
| `amortizationType.refName` | Reference Name | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `initialAmount` | Initial Amount | number | double |  |  |  |
| `isAmortization` | Is Amortization | boolean |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `isPublic` | Public | boolean |  |  |  |  |
| `isSchedule` | Is Schedule | boolean |  |  |  |  |
| `job` |  | job |  |  | [`job`](job.md#job) |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Name | string |  |  |  |  |
| `periodOffset` | Period Offset | integer | int64 |  |  |  |
| `recogIntervalSrc` |  | object |  |  |  |  |
| `recogIntervalSrc.id` | Internal identifier | string |  |  |  | `RECEIPTDATE`, `USERDEFINED`, `BETWEENBILLS`, `BETWEENBILLSRRDATE`, `SOREVRECDATES` |
| `recogIntervalSrc.refName` | Reference Name | string |  |  |  |  |
| `recurrence` |  | revRecTemplate-recurrenceCollection |  |  | [`revRecTemplate-recurrenceCollection`](#revrectemplate-recurrencecollection) |  |
| `recurrenceType` |  | object |  |  |  |  |
| `recurrenceType.id` | Internal identifier | string |  |  |  | `DATESPRORATE`, `EVENPERIODSPRORATE`, `CUSTOM`, `EVENPRORATEPERIOD`, `DATESINTOPERIODS` |
| `recurrenceType.refName` | Reference Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revRecNumber` | Rev Rec Number | string |  |  |  |  |
| `revRecOffset` | Start Offset | integer | int64 |  |  |  |
| `target` | Target | string |  |  |  |  |
| `totalAmount` | Amount | number | double |  |  |  |

## revRecTemplate-recurrenceCollection

Browser definition `revRecTemplate-recurrenceCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | revRecTemplate-recurrenceElement[] |  |  | [`revRecTemplate-recurrenceElement`](#revrectemplate-recurrenceelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## revRecTemplate-recurrenceElement

Browser definition `revRecTemplate-recurrenceElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `defRevAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `incomeAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `periodOffset` | Period Offset | integer | int64 |  |  |  |
| `postingPeriod` |  | string |  |  |  |  |
| `recAmount` | Amount | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## revRecTemplateCollection

Browser definition `revRecTemplateCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | revRecTemplate[] |  |  | [`revRecTemplate`](#revrectemplate) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## revRecTemplateSelectOptions

Browser definition `revRecTemplateSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amortizationType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `job` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `recogIntervalSrc` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `recurrenceType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
