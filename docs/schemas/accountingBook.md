# Schemas: accountingBook

Property tables for definitions owned by `accountingBook`.

Record page: [accountingBook](../records/accountingBook.md).

## Index

- [accountingBook](#accountingbook) — 26 properties
- [accountingBook-accountingBookSubsidiariesCollection](#accountingbook-accountingbooksubsidiariescollection) — 6 properties
- [accountingBook-accountingBookSubsidiariesElement](#accountingbook-accountingbooksubsidiarieselement) — 11 properties
- [accountingBookCollection](#accountingbookcollection) — 6 properties
- [accountingBookSelectOptions](#accountingbookselectoptions) — 7 properties

## accountingBook

Browser definition `accountingBook`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBookSubsidiaries` |  | accountingBook-accountingBookSubsidiariesCollection |  |  | [`accountingBook-accountingBookSubsidiariesCollection`](#accountingbook-accountingbooksubsidiariescollection) |  |
| `baseBook` |  | accountingBook |  |  | [`accountingBook`](#accountingbook) |  |
| `contingentRevenueHandling` | Enable contingent revenue handling | boolean |  |  |  |  |
| `createdDate` | Created Date | string | date-time |  |  |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `effectivePeriod` |  | accountingPeriod |  |  | [`accountingPeriod`](accountingPeriod.md#accountingperiod) |  |
| `externalId` | External ID | string |  |  |  |  |
| `firstBasePeriod` |  | accountingPeriod |  |  | [`accountingPeriod`](accountingPeriod.md#accountingperiod) |  |
| `id` | Internal ID | string |  |  |  |  |
| `includeChildren` | Include Children | boolean |  |  |  |  |
| `isAdjustmentOnly` | Adjustment Only | boolean |  |  |  |  |
| `isConsolidated` | Enable Consolidation | boolean |  |  |  |  |
| `isPrimary` | Is Primary | boolean |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `status` |  | object |  |  |  |  |
| `status.id` | Internal identifier | string |  |  |  | `ACTIVE`, `INACTIVE`, `PENDING` |
| `status.refName` | Reference Name | string |  |  |  |  |
| `subsidiariesString` | Subsidiaries | string |  |  |  |  |
| `subsidiary` |  | subsidiaryCollection |  |  | [`subsidiaryCollection`](subsidiary.md#subsidiarycollection) |  |
| `twoStepRevenueAllocation` | Enable two step revenue allocation | boolean |  |  |  |  |
| `unbilledReceivableGrouping` |  | object |  |  |  |  |
| `unbilledReceivableGrouping.id` | Internal identifier | string |  |  |  | `SUBARRANGEMENTGROUP`, `ELEMENT`, `ARRANGEMENT` |
| `unbilledReceivableGrouping.refName` | Reference Name | string |  |  |  |  |

## accountingBook-accountingBookSubsidiariesCollection

Browser definition `accountingBook-accountingBookSubsidiariesCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | accountingBook-accountingBookSubsidiariesElement[] |  |  | [`accountingBook-accountingBookSubsidiariesElement`](#accountingbook-accountingbooksubsidiarieselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## accountingBook-accountingBookSubsidiariesElement

Browser definition `accountingBook-accountingBookSubsidiariesElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `effectiveDate` | Effective Date | string | date |  |  |  |
| `enablePeriodEndJournals` | Enable Period End Journal Entries | boolean |  |  |  |  |
| `exchangeRate` | Translation Exchange Rate | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `primaryBookCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `status` |  | object |  |  |  |  |
| `status.id` | Internal identifier | string |  |  |  | `ACTIVE`, `INACTIVE`, `PENDING` |
| `status.refName` | Reference Name | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |

## accountingBookCollection

Browser definition `accountingBookCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | accountingBook[] |  |  | [`accountingBook`](#accountingbook) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## accountingBookSelectOptions

Browser definition `accountingBookSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `baseBook` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `effectivePeriod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `firstBasePeriod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `status` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `unbilledReceivableGrouping` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
