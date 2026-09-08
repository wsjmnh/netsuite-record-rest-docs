# Schemas: journalEntry

Property tables for definitions owned by `journalEntry`.

Record page: [journalEntry](../records/journalEntry.md).

## Index

- [journalEntry](#journalentry) — 47 properties
- [journalEntry-accountingBookDetailCollection](#journalentry-accountingbookdetailcollection) — 6 properties
- [journalEntry-accountingBookDetailElement](#journalentry-accountingbookdetailelement) — 7 properties
- [journalEntry-appliedRulesCollection](#journalentry-appliedrulescollection) — 6 properties
- [journalEntry-appliedRulesElement](#journalentry-appliedruleselement) — 9 properties
- [journalEntry-lineCollection](#journalentry-linecollection) — 6 properties
- [journalEntry-lineElement](#journalentry-lineelement) — 41 properties
- [journalEntryCollection](#journalentrycollection) — 6 properties
- [journalEntrySelectOptions](#journalentryselectoptions) — 18 properties

## journalEntry

Browser definition `journalEntry`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | accountingBook |  |  | [`accountingBook`](accountingBook.md#accountingbook) |  |
| `accountingBookDetail` |  | journalEntry-accountingBookDetailCollection |  |  | [`journalEntry-accountingBookDetailCollection`](#journalentry-accountingbookdetailcollection) |  |
| `appliedRules` |  | journalEntry-appliedRulesCollection |  |  | [`journalEntry-appliedRulesCollection`](#journalentry-appliedrulescollection) |  |
| `approvalStatus` |  | object |  |  |  |  |
| `approvalStatus.id` | Internal identifier | string |  |  |  | `11`, `1`, `2`, `3` |
| `approvalStatus.refName` | Reference Name | string |  |  |  |  |
| `approved` | Approved | boolean |  |  |  |  |
| `batch` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `createdFrom` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReason` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReasonMemo` | Deletion Reason Memo | string |  |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `excludeFromGLNumbering` | Exclude from GL Audit Numbering | boolean |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isBookSpecific` | Is Book Specific | boolean |  |  |  |  |
| `isReversal` | Is Reversal | boolean |  |  |  |  |
| `lastModifiedDate` | Date Last Modified | string | date-time |  |  |  |
| `line` |  | journalEntry-lineCollection |  |  | [`journalEntry-lineCollection`](#journalentry-linecollection) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `nextApprover` |  | employee |  |  | [`employee`](employee.md#employee) |  |
| `nexus` |  | nexus |  |  | [`nexus`](nexus.md#nexus) |  |
| `parentExpenseAlloc` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `postingPeriod` |  | accountingPeriod |  |  | [`accountingPeriod`](accountingPeriod.md#accountingperiod) |  |
| `primaryBookBaseCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `reversalDate` | Reversal Date | string | date |  |  |  |
| `reversalDefer` | Defer Entry | boolean |  |  |  |  |
| `reversalEntry` | Reversal No. | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `subsidiaryTaxRegNum` | Subsidiary Tax Reg. Number | string |  |  |  |  |
| `taxDetailsOverride` | Tax Details Override | boolean |  |  |  |  |
| `taxPointDate` | Tax Point Date | string | date |  |  |  |
| `taxPointDateOverride` | Tax Point Date Override | boolean |  |  |  |  |
| `taxRegOverride` | Tax Registration Override | boolean |  |  |  |  |
| `toSubsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `tranDate` | Date | string | date |  |  |  |
| `tranId` | Entry No. | string |  |  |  |  |
| `transactionNumber` | Transaction Number | string |  |  |  |  |
| `void` | Void | boolean |  |  |  |  |

## journalEntry-accountingBookDetailCollection

Browser definition `journalEntry-accountingBookDetailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | journalEntry-accountingBookDetailElement[] |  |  | [`journalEntry-accountingBookDetailElement`](#journalentry-accountingbookdetailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## journalEntry-accountingBookDetailElement

Browser definition `journalEntry-accountingBookDetailElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | accountingBook |  |  | [`accountingBook`](accountingBook.md#accountingbook) |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revRecOnRevCommitment` | Rev Rec on Rev Commit. | boolean |  |  |  |  |
| `tranIsVsoeBundle` | Transaction Is VSOE Bundle | boolean |  |  |  |  |

## journalEntry-appliedRulesCollection

Browser definition `journalEntry-appliedRulesCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | journalEntry-appliedRulesElement[] |  |  | [`journalEntry-appliedRulesElement`](#journalentry-appliedruleselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## journalEntry-appliedRulesElement

Browser definition `journalEntry-appliedRulesElement`.

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

## journalEntry-lineCollection

Browser definition `journalEntry-lineCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | journalEntry-lineElement[] |  |  | [`journalEntry-lineElement`](#journalentry-lineelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## journalEntry-lineElement

Browser definition `journalEntry-lineElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | account |  |  | [`account`](account.md#account) |  |
| `amortizationType` | Type | string |  |  |  |  |
| `baseGrossAmt` | Gross Amount | number | double |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `cleared` | Cleared | boolean |  |  |  |  |
| `clearedDate` | Date Cleared | string | date |  |  |  |
| `credit` | Credit | number | double |  |  |  |
| `creditTax` | Credit Tax | number | double |  |  |  |
| `debit` | Debit | number | double |  |  |  |
| `debitTax` | Debit Tax | number | double |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `eliminate` | Eliminate | boolean |  |  |  |  |
| `endDate` | End Date | string | date |  |  |  |
| `entity` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `giftCertCode` |  | giftCertificate |  |  | [`giftCertificate`](giftCertificate.md#giftcertificate) |  |
| `grossAmt` | Gross Amt | number | double |  |  |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `line` | Line Id | integer | int64 |  |  |  |
| `lineCreatedDate` | Line Created Date | string | date-time |  |  |  |
| `lineLastModifiedDate` | Line Last Modified Date | string | date-time |  |  |  |
| `lineTaxCode` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `lineTaxRate` | Tax Rate | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `residual` | Residual | number | double |  |  |  |
| `revenueRecognitionRule` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `schedule` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `scheduleNum` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `scheduleType` |  | object |  |  |  |  |
| `scheduleType.id` | Internal identifier | string |  |  |  | `Amortization`, `RevRec` |
| `scheduleType.refName` | Reference Name | string |  |  |  |  |
| `startDate` | Start Date | string | date |  |  |  |
| `tax1Acct` |  | account |  |  | [`account`](account.md#account) |  |
| `tax1Amt` | Tax Amt | number | double |  |  |  |
| `taxAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `taxBasis` | Tax Basis | number | double |  |  |  |
| `taxCode` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `taxRate1` | Tax Rate | number | double |  |  |  |
| `totalAmount` | Total Amount | number | double |  |  |  |

## journalEntryCollection

Browser definition `journalEntryCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | journalEntry[] |  |  | [`journalEntry`](#journalentry) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## journalEntrySelectOptions

Browser definition `journalEntrySelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `approvalStatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `batch` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `createdFrom` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `currency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deletionReason` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `nextApprover` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `nexus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `parentExpenseAlloc` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `postingPeriod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `primaryBookBaseCurrency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiaryTaxRegNum` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `toSubsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
