# Schemas: advIntercompanyJournalEntry

Property tables for definitions owned by `advIntercompanyJournalEntry`.

Record page: [advIntercompanyJournalEntry](../records/advIntercompanyJournalEntry.md).

## Index

- [advIntercompanyJournalEntry](#advintercompanyjournalentry) — 41 properties
- [advIntercompanyJournalEntry-accountingBookDetailCollection](#advintercompanyjournalentry-accountingbookdetailcollection) — 6 properties
- [advIntercompanyJournalEntry-accountingBookDetailElement](#advintercompanyjournalentry-accountingbookdetailelement) — 8 properties
- [advIntercompanyJournalEntry-appliedRulesCollection](#advintercompanyjournalentry-appliedrulescollection) — 6 properties
- [advIntercompanyJournalEntry-appliedRulesElement](#advintercompanyjournalentry-appliedruleselement) — 9 properties
- [advIntercompanyJournalEntry-lineCollection](#advintercompanyjournalentry-linecollection) — 6 properties
- [advIntercompanyJournalEntry-lineElement](#advintercompanyjournalentry-lineelement) — 49 properties
- [advIntercompanyJournalEntryCollection](#advintercompanyjournalentrycollection) — 6 properties
- [advIntercompanyJournalEntrySelectOptions](#advintercompanyjournalentryselectoptions) — 16 properties

## advIntercompanyJournalEntry

Browser definition `advIntercompanyJournalEntry`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | accountingBook |  |  | [`accountingBook`](accountingBook.md#accountingbook) |  |
| `accountingBookDetail` |  | advIntercompanyJournalEntry-accountingBookDetailCollection |  |  | [`advIntercompanyJournalEntry-accountingBookDetailCollection`](#advintercompanyjournalentry-accountingbookdetailcollection) |  |
| `appliedRules` |  | advIntercompanyJournalEntry-appliedRulesCollection |  |  | [`advIntercompanyJournalEntry-appliedRulesCollection`](#advintercompanyjournalentry-appliedrulescollection) |  |
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
| `excludeFromGLNumbering` | Exclude from GL Audit Numbering | boolean |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isBookSpecific` | Is Book Specific | boolean |  |  |  |  |
| `isReversal` | Is Reversal | boolean |  |  |  |  |
| `lastModifiedDate` | Date Last Modified | string | date-time |  |  |  |
| `line` |  | advIntercompanyJournalEntry-lineCollection |  |  | [`advIntercompanyJournalEntry-lineCollection`](#advintercompanyjournalentry-linecollection) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `nextApprover` |  | employee |  |  | [`employee`](employee.md#employee) |  |
| `nexus` |  | nexus |  |  | [`nexus`](nexus.md#nexus) |  |
| `parentExpenseAlloc` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `performAutoBalance` | Perform Auto Balance | boolean |  |  |  |  |
| `postingPeriod` |  | accountingPeriod |  |  | [`accountingPeriod`](accountingPeriod.md#accountingperiod) |  |
| `prevDate` | Previous Effective Date | string | date |  |  |  |
| `primaryBookBaseCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `reversalDate` | Reversal Date | string | date |  |  |  |
| `reversalDefer` | Defer Entry | boolean |  |  |  |  |
| `reversalEntry` | Reversal No. | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `toSubsidiaries` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `tranDate` | Date | string | date |  |  |  |
| `tranId` | Entry No. | string |  |  |  |  |
| `transactionNumber` | Transaction Number | string |  |  |  |  |

## advIntercompanyJournalEntry-accountingBookDetailCollection

Browser definition `advIntercompanyJournalEntry-accountingBookDetailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | advIntercompanyJournalEntry-accountingBookDetailElement[] |  |  | [`advIntercompanyJournalEntry-accountingBookDetailElement`](#advintercompanyjournalentry-accountingbookdetailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## advIntercompanyJournalEntry-accountingBookDetailElement

Browser definition `advIntercompanyJournalEntry-accountingBookDetailElement`.

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

## advIntercompanyJournalEntry-appliedRulesCollection

Browser definition `advIntercompanyJournalEntry-appliedRulesCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | advIntercompanyJournalEntry-appliedRulesElement[] |  |  | [`advIntercompanyJournalEntry-appliedRulesElement`](#advintercompanyjournalentry-appliedruleselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## advIntercompanyJournalEntry-appliedRulesElement

Browser definition `advIntercompanyJournalEntry-appliedRulesElement`.

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

## advIntercompanyJournalEntry-lineCollection

Browser definition `advIntercompanyJournalEntry-lineCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | advIntercompanyJournalEntry-lineElement[] |  |  | [`advIntercompanyJournalEntry-lineElement`](#advintercompanyjournalentry-lineelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## advIntercompanyJournalEntry-lineElement

Browser definition `advIntercompanyJournalEntry-lineElement`.

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
| `dueToFromSubsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `eliminate` | Eliminate | boolean |  |  |  |  |
| `endDate` | End Date | string | date |  |  |  |
| `entity` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `entityrepresentssubsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `giftCertCode` |  | giftCertificate |  |  | [`giftCertificate`](giftCertificate.md#giftcertificate) |  |
| `grossAmt` | Gross Amt | number | double |  |  |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `line` | Line Id | integer | int64 |  |  |  |
| `lineBaseCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `lineCreatedDate` | Line Created Date | string | date-time |  |  |  |
| `lineCurrencyPrecision` | Currency Precision | string |  |  |  |  |
| `lineFxRate` | Exchange Rate | number | double |  |  |  |
| `lineLastModifiedDate` | Line Last Modified Date | string | date-time |  |  |  |
| `lineSubsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `lineTaxCode` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `lineTaxRate` | Tax Rate | number | double |  |  |  |
| `lineTotalAmt` | Total Amount (Base Currency) | number | double |  |  |  |
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

## advIntercompanyJournalEntryCollection

Browser definition `advIntercompanyJournalEntryCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | advIntercompanyJournalEntry[] |  |  | [`advIntercompanyJournalEntry`](#advintercompanyjournalentry) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## advIntercompanyJournalEntrySelectOptions

Browser definition `advIntercompanyJournalEntrySelectOptions`.

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
| `toSubsidiaries` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
