# Schemas: depositApplication

Property tables for definitions owned by `depositApplication`.

Record page: [depositApplication](../records/depositApplication.md).

## Index

- [depositApplication](#depositapplication) — 36 properties
- [depositApplication-accountingBookDetailCollection](#depositapplication-accountingbookdetailcollection) — 6 properties
- [depositApplication-accountingBookDetailElement](#depositapplication-accountingbookdetailelement) — 7 properties
- [depositApplication-appliedRulesCollection](#depositapplication-appliedrulescollection) — 6 properties
- [depositApplication-appliedRulesElement](#depositapplication-appliedruleselement) — 9 properties
- [depositApplication-applyCollection](#depositapplication-applycollection) — 6 properties
- [depositApplication-applyElement](#depositapplication-applyelement) — 15 properties
- [depositApplicationCollection](#depositapplicationcollection) — 6 properties
- [depositApplicationSelectOptions](#depositapplicationselectoptions) — 13 properties

## depositApplication

Browser definition `depositApplication`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBookDetail` |  | depositApplication-accountingBookDetailCollection |  |  | [`depositApplication-accountingBookDetailCollection`](#depositapplication-accountingbookdetailcollection) |  |
| `applied` | Applied | number | double |  |  |  |
| `appliedRules` |  | depositApplication-appliedRulesCollection |  |  | [`depositApplication-appliedRulesCollection`](#depositapplication-appliedrulescollection) |  |
| `apply` |  | depositApplication-applyCollection |  |  | [`depositApplication-applyCollection`](#depositapplication-applycollection) |  |
| `arAcct` |  | account |  |  | [`account`](account.md#account) |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `customer` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `deletionReason` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReasonMemo` | Deletion Reason Memo | string |  |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `deposit` |  | customerDeposit |  |  | [`customerDeposit`](customerDeposit.md#customerdeposit) |  |
| `depositDate` | Deposit Date | string | date |  |  |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `excludeFromGLNumbering` | Exclude from GL Audit Numbering | boolean |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `lastModifiedDate` | Date Last Modified | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `postingPeriod` |  | accountingPeriod |  |  | [`accountingPeriod`](accountingPeriod.md#accountingperiod) |  |
| `prevDate` | Previous Effective Date | string | date |  |  |  |
| `primaryBookBaseCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `status` |  | object |  |  |  |  |
| `status.id` | Internal identifier | string |  |  |  |  |
| `status.refName` | Reference Name | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `total` | To Apply | number | double |  |  |  |
| `tranDate` | Date | string | date |  |  |  |
| `tranId` | Deposit Application # | string |  |  |  |  |
| `transactionNumber` | Transaction Number | string |  |  |  |  |
| `unapplied` | Unapplied | number | double |  |  |  |

## depositApplication-accountingBookDetailCollection

Browser definition `depositApplication-accountingBookDetailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | depositApplication-accountingBookDetailElement[] |  |  | [`depositApplication-accountingBookDetailElement`](#depositapplication-accountingbookdetailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## depositApplication-accountingBookDetailElement

Browser definition `depositApplication-accountingBookDetailElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | accountingBook |  |  | [`accountingBook`](accountingBook.md#accountingbook) |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revRecOnRevCommitment` | Rev Rec on Rev Commit. | boolean |  |  |  |  |
| `tranIsVsoeBundle` | Transaction Is VSOE Bundle | boolean |  |  |  |  |

## depositApplication-appliedRulesCollection

Browser definition `depositApplication-appliedRulesCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | depositApplication-appliedRulesElement[] |  |  | [`depositApplication-appliedRulesElement`](#depositapplication-appliedruleselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## depositApplication-appliedRulesElement

Browser definition `depositApplication-appliedRulesElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `creationDate` | Date | string | date |  |  |  |
| `details` | Details | string |  |  |  |  |
| `externalLogId` | External ID | integer | int64 |  |  |  |
| `id` | ID | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `ruleType` | Rule Type: | string |  |  |  |  |
| `ruleTypeTranslation` | Rule Type | string |  |  |  |  |
| `transactionVersion` | Version | integer | int64 |  |  |  |

## depositApplication-applyCollection

Browser definition `depositApplication-applyCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | depositApplication-applyElement[] |  |  | [`depositApplication-applyElement`](#depositapplication-applyelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## depositApplication-applyElement

Browser definition `depositApplication-applyElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amount` | Payment | number | double |  |  |  |
| `apply` | Apply | boolean |  |  |  |  |
| `applyDate` | Date | string | date |  |  |  |
| `createdFrom` | Created From | string |  |  |  |  |
| `currency` | Currency | string |  |  |  |  |
| `doc` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `due` | Amt. Due | number | double |  |  |  |
| `job` | Job ID | integer | int64 |  |  |  |
| `jobName` | Subcustomer | string |  |  |  |  |
| `line` | Line Id | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `refNum` | Ref No. | string |  |  |  |  |
| `total` | Orig. Amt. | number | double |  |  |  |
| `type` | Type | string |  |  |  |  |

## depositApplicationCollection

Browser definition `depositApplicationCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | depositApplication[] |  |  | [`depositApplication`](#depositapplication) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## depositApplicationSelectOptions

Browser definition `depositApplicationSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `arAcct` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `currency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customer` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deletionReason` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deposit` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `postingPeriod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `primaryBookBaseCurrency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `status` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
