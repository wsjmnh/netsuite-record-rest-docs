# Schemas: intercompanyJournalEntry

Property tables for definitions owned by `intercompanyJournalEntry`.

Record page: [intercompanyJournalEntry](../records/intercompanyJournalEntry.md).

## Index

- [intercompanyJournalEntry](#intercompanyjournalentry) — 41 properties
- [intercompanyJournalEntry-accountingBookDetailCollection](#intercompanyjournalentry-accountingbookdetailcollection) — 6 properties
- [intercompanyJournalEntry-accountingBookDetailElement](#intercompanyjournalentry-accountingbookdetailelement) — 8 properties
- [intercompanyJournalEntry-appliedRulesCollection](#intercompanyjournalentry-appliedrulescollection) — 6 properties
- [intercompanyJournalEntry-appliedRulesElement](#intercompanyjournalentry-appliedruleselement) — 9 properties
- [intercompanyJournalEntry-lineCollection](#intercompanyjournalentry-linecollection) — 6 properties
- [intercompanyJournalEntry-lineElement](#intercompanyjournalentry-lineelement) — 43 properties
- [intercompanyJournalEntryCollection](#intercompanyjournalentrycollection) — 6 properties
- [intercompanyJournalEntrySelectOptions](#intercompanyjournalentryselectoptions) — 16 properties

## intercompanyJournalEntry

Browser definition `intercompanyJournalEntry`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | accountingBook |  |  | [`accountingBook`](accountingBook.md#accountingbook) |  |
| `accountingBookDetail` |  | intercompanyJournalEntry-accountingBookDetailCollection |  |  | [`intercompanyJournalEntry-accountingBookDetailCollection`](#intercompanyjournalentry-accountingbookdetailcollection) |  |
| `appliedRules` |  | intercompanyJournalEntry-appliedRulesCollection |  |  | [`intercompanyJournalEntry-appliedRulesCollection`](#intercompanyjournalentry-appliedrulescollection) |  |
| `approvalStatus` |  | object |  |  |  |  |
| `approvalStatus.id` | Internal identifier | string |  |  |  | `11`, `1`, `2`, `3` |
| `approvalStatus.refName` | Reference Name | string |  |  |  |  |
| `approved` | Approved | boolean |  |  |  |  |
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
| `line` |  | intercompanyJournalEntry-lineCollection |  |  | [`intercompanyJournalEntry-lineCollection`](#intercompanyjournalentry-linecollection) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `nextApprover` |  | employee |  |  | [`employee`](employee.md#employee) |  |
| `nexus` |  | nexus |  |  | [`nexus`](nexus.md#nexus) |  |
| `parentExpenseAlloc` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `postingPeriod` |  | accountingPeriod |  |  | [`accountingPeriod`](accountingPeriod.md#accountingperiod) |  |
| `prevDate` | Previous Effective Date | string | date |  |  |  |
| `primaryBookBaseCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `reversalDate` | Reversal Date | string | date |  |  |  |
| `reversalDefer` | Defer Entry | boolean |  |  |  |  |
| `reversalEntry` | Reversal No. | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `toSubsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `tranDate` | Date | string | date |  |  |  |
| `tranId` | Entry No. | string |  |  |  |  |
| `transactionNumber` | Transaction Number | string |  |  |  |  |

## intercompanyJournalEntry-accountingBookDetailCollection

Browser definition `intercompanyJournalEntry-accountingBookDetailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | intercompanyJournalEntry-accountingBookDetailElement[] |  |  | [`intercompanyJournalEntry-accountingBookDetailElement`](#intercompanyjournalentry-accountingbookdetailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## intercompanyJournalEntry-accountingBookDetailElement

Browser definition `intercompanyJournalEntry-accountingBookDetailElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | accountingBook |  |  | [`accountingBook`](accountingBook.md#accountingbook) |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revRecOnRevCommitment` | Rev Rec on Rev Commit. | boolean |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `tranIsVsoeBundle` | Transaction Is VSOE Bundle | boolean |  |  |  |  |

## intercompanyJournalEntry-appliedRulesCollection

Browser definition `intercompanyJournalEntry-appliedRulesCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | intercompanyJournalEntry-appliedRulesElement[] |  |  | [`intercompanyJournalEntry-appliedRulesElement`](#intercompanyjournalentry-appliedruleselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## intercompanyJournalEntry-appliedRulesElement

Browser definition `intercompanyJournalEntry-appliedRulesElement`.

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

## intercompanyJournalEntry-lineCollection

Browser definition `intercompanyJournalEntry-lineCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | intercompanyJournalEntry-lineElement[] |  |  | [`intercompanyJournalEntry-lineElement`](#intercompanyjournalentry-lineelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## intercompanyJournalEntry-lineElement

Browser definition `intercompanyJournalEntry-lineElement`.

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
| `lineSubsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
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
| `taxDetailsReference` | Tax Details Reference | string |  |  |  |  |
| `taxRate1` | Tax Rate | number | double |  |  |  |
| `totalAmount` | Total Amount | number | double |  |  |  |

## intercompanyJournalEntryCollection

Browser definition `intercompanyJournalEntryCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | intercompanyJournalEntry[] |  |  | [`intercompanyJournalEntry`](#intercompanyjournalentry) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## intercompanyJournalEntrySelectOptions

Browser definition `intercompanyJournalEntrySelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `approvalStatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
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
| `toSubsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
