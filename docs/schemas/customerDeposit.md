# Schemas: customerDeposit

Property tables for definitions owned by `customerDeposit`.

Record page: [customerDeposit](../records/customerDeposit.md).

## Index

- [customerDeposit](#customerdeposit) — 67 properties
- [customerDeposit-accountingBookDetailCollection](#customerdeposit-accountingbookdetailcollection) — 6 properties
- [customerDeposit-accountingBookDetailElement](#customerdeposit-accountingbookdetailelement) — 7 properties
- [customerDeposit-appliedRulesCollection](#customerdeposit-appliedrulescollection) — 6 properties
- [customerDeposit-appliedRulesElement](#customerdeposit-appliedruleselement) — 9 properties
- [customerDepositCollection](#customerdepositcollection) — 6 properties
- [customerDepositSelectOptions](#customerdepositselectoptions) — 22 properties

## customerDeposit

Browser definition `customerDeposit`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | account |  |  | [`account`](account.md#account) |  |
| `accountingBookDetail` |  | customerDeposit-accountingBookDetailCollection |  |  | [`customerDeposit-accountingBookDetailCollection`](#customerdeposit-accountingbookdetailcollection) |  |
| `appliedRules` |  | customerDeposit-appliedRulesCollection |  |  | [`customerDeposit-appliedRulesCollection`](#customerdeposit-appliedrulescollection) |  |
| `cardSwipe` | Card Swipe | string |  |  |  |  |
| `cardholderAuthentication` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `checkNumber` | Check # | string |  |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `cleared` | Cleared | boolean |  |  |  |  |
| `clearedDate` | Date Cleared | string | date |  |  |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `customer` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `customerPaymentAuthorization` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `debitKsn` | Debit KSN | string |  |  |  |  |
| `debitPinBlock` | Debit Pin Block | string |  |  |  |  |
| `deletionReason` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReasonMemo` | Deletion Reason Memo | string |  |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `depositSufficient` | Deposit Sufficient | boolean |  |  |  |  |
| `dynamicDescriptor` | Soft Descriptor | string |  |  |  |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `excludeFromGLNumbering` | Exclude from GL Audit Numbering | boolean |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `handlingMode` |  | object |  |  |  |  |
| `handlingMode.id` | Internal identifier | string |  |  |  | `MIMIC`, `PROCESS`, `SAVE_ONLY` |
| `handlingMode.refName` | Reference Name | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `inputReferenceCode` | Input P/N Ref. | string |  |  |  |  |
| `integrationId` | Integration ID | string |  |  |  |  |
| `lastModifiedDate` | Date Last Modified | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `nexus` |  | nexus |  |  | [`nexus`](nexus.md#nexus) |  |
| `outputAuthCode` | Auth. Code | string |  |  |  |  |
| `outputReferenceCode` | P/N Ref. | string |  |  |  |  |
| `payment` | Payment Amount | number | double |  |  |  |
| `paymentCardCsc` | CSC | string |  |  |  |  |
| `paymentDeviceId` | Payment Device ID | string |  |  |  |  |
| `paymentInstrumentLimit` | Payment Instrument Limit | number | double |  |  |  |
| `paymentOperation` |  | object |  |  |  |  |
| `paymentOperation.id` | Internal identifier | string |  |  |  | `SALE`, `CAPTURE` |
| `paymentOperation.refName` | Reference Name | string |  |  |  |  |
| `paymentOption` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `paymentProcessingProfile` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `postingPeriod` |  | accountingPeriod |  |  | [`accountingPeriod`](accountingPeriod.md#accountingperiod) |  |
| `prevDate` | Previous Effective Date | string | date |  |  |  |
| `primaryBookBaseCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `refundedAmountTotalBox` | Refunded | number | double |  |  |  |
| `salesOrder` |  | salesOrder |  |  | [`salesOrder`](salesOrder.md#salesorder) |  |
| `salesOrderRequiredDepositDue` | Sales Order Required Deposit Due | number | double |  |  |  |
| `salesOrderUnpaidAmount` | Sales Order Unpaid Amount | number | double |  |  |  |
| `status` |  | object |  |  |  |  |
| `status.id` | Internal identifier | string |  |  |  | `A`, `B`, `R`, `C`, `D` |
| `status.refName` | Reference Name | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `toBeEmailed` | To Be Emailed | boolean |  |  |  |  |
| `total` | Total | number | double |  |  |  |
| `tranDate` | Date | string | date |  |  |  |
| `tranId` | Deposit # | string |  |  |  |  |
| `transactionNumber` | Transaction Number | string |  |  |  |  |
| `transactionToRefund` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `undepFunds` |  | object |  |  |  |  |
| `undepFunds.id` | Internal identifier | string |  |  |  |  |
| `undepFunds.refName` | Reference Name | string |  |  |  |  |

## customerDeposit-accountingBookDetailCollection

Browser definition `customerDeposit-accountingBookDetailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | customerDeposit-accountingBookDetailElement[] |  |  | [`customerDeposit-accountingBookDetailElement`](#customerdeposit-accountingbookdetailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## customerDeposit-accountingBookDetailElement

Browser definition `customerDeposit-accountingBookDetailElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | accountingBook |  |  | [`accountingBook`](accountingBook.md#accountingbook) |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revRecOnRevCommitment` | Rev Rec on Rev Commit. | boolean |  |  |  |  |
| `tranIsVsoeBundle` | Transaction Is VSOE Bundle | boolean |  |  |  |  |

## customerDeposit-appliedRulesCollection

Browser definition `customerDeposit-appliedRulesCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | customerDeposit-appliedRulesElement[] |  |  | [`customerDeposit-appliedRulesElement`](#customerdeposit-appliedruleselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## customerDeposit-appliedRulesElement

Browser definition `customerDeposit-appliedRulesElement`.

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

## customerDepositCollection

Browser definition `customerDepositCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | customerDeposit[] |  |  | [`customerDeposit`](#customerdeposit) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## customerDepositSelectOptions

Browser definition `customerDepositSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `cardholderAuthentication` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `currency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customer` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customerPaymentAuthorization` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deletionReason` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `handlingMode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `nexus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `paymentOperation` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `paymentOption` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `paymentProcessingProfile` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `postingPeriod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `primaryBookBaseCurrency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `salesOrder` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `status` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `transactionToRefund` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `undepFunds` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
