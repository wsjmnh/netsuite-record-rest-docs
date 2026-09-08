# Schemas: vendorPrepaymentApplication

Property tables for definitions owned by `vendorPrepaymentApplication`.

Record page: [vendorPrepaymentApplication](../records/vendorPrepaymentApplication.md).

## Index

- [vendorPrepaymentApplication](#vendorprepaymentapplication) — 29 properties
- [vendorPrepaymentApplication-billCollection](#vendorprepaymentapplication-billcollection) — 6 properties
- [vendorPrepaymentApplication-billElement](#vendorprepaymentapplication-billelement) — 13 properties
- [vendorPrepaymentApplicationCollection](#vendorprepaymentapplicationcollection) — 6 properties
- [vendorPrepaymentApplicationSelectOptions](#vendorprepaymentapplicationselectoptions) — 11 properties

## vendorPrepaymentApplication

Browser definition `vendorPrepaymentApplication`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | account |  |  | [`account`](account.md#account) |  |
| `applied` | Applied | number | double |  |  |  |
| `bill` |  | vendorPrepaymentApplication-billCollection |  |  | [`vendorPrepaymentApplication-billCollection`](#vendorprepaymentapplication-billcollection) |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReason` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReasonMemo` | Deletion Reason Memo | string |  |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `entity` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `lastModifiedDate` | Date Last Modified | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `postingPeriod` |  | accountingPeriod |  |  | [`accountingPeriod`](accountingPeriod.md#accountingperiod) |  |
| `prepaymentDate` | Prepayment Date | string | date |  |  |  |
| `prevDate` | Previous Effective Date | string | date |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `total` | Total | number | double |  |  |  |
| `tranDate` | Date | string | date |  |  |  |
| `tranId` | Document Number | string |  |  |  |  |
| `transactionNumber` | Transaction Number | string |  |  |  |  |
| `unapplied` | Unapplied | number | double |  |  |  |
| `vendorPrepayment` |  | vendorPrepayment |  |  | [`vendorPrepayment`](vendorPrepayment.md#vendorprepayment) |  |

## vendorPrepaymentApplication-billCollection

Browser definition `vendorPrepaymentApplication-billCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | vendorPrepaymentApplication-billElement[] |  |  | [`vendorPrepaymentApplication-billElement`](#vendorprepaymentapplication-billelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## vendorPrepaymentApplication-billElement

Browser definition `vendorPrepaymentApplication-billElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amount` | Payment | number | double |  |  |  |
| `apply` | Apply | boolean |  |  |  |  |
| `applyDate` | Date | string | date |  |  |  |
| `createdFrom` | Created From | string |  |  |  |  |
| `currency` | Currency | string |  |  |  |  |
| `doc` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `due` | Amt. Due | number | double |  |  |  |
| `line` | Line Id | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `refNum` | Ref No. | string |  |  |  |  |
| `total` | Orig. Amt. | number | double |  |  |  |
| `type` | Type | string |  |  |  |  |

## vendorPrepaymentApplicationCollection

Browser definition `vendorPrepaymentApplicationCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | vendorPrepaymentApplication[] |  |  | [`vendorPrepaymentApplication`](#vendorprepaymentapplication) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## vendorPrepaymentApplicationSelectOptions

Browser definition `vendorPrepaymentApplicationSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `currency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deletionReason` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `entity` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `postingPeriod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `vendorPrepayment` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
