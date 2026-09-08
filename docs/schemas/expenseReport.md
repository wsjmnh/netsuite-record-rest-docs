# Schemas: expenseReport

Property tables for definitions owned by `expenseReport`.

Record page: [expenseReport](../records/expenseReport.md).

## Index

- [expenseReport](#expensereport) — 62 properties
- [expenseReport-accountingBookDetailCollection](#expensereport-accountingbookdetailcollection) — 6 properties
- [expenseReport-accountingBookDetailElement](#expensereport-accountingbookdetailelement) — 7 properties
- [expenseReport-appliedRulesCollection](#expensereport-appliedrulescollection) — 6 properties
- [expenseReport-appliedRulesElement](#expensereport-appliedruleselement) — 9 properties
- [expenseReport-expenseCollection](#expensereport-expensecollection) — 6 properties
- [expenseReport-expenseElement](#expensereport-expenseelement) — 36 properties
- [expenseReport-taxDetailsCollection](#expensereport-taxdetailscollection) — 6 properties
- [expenseReport-taxDetailsElement](#expensereport-taxdetailselement) — 14 properties
- [expenseReportCollection](#expensereportcollection) — 6 properties
- [expenseReportSelectOptions](#expensereportselectoptions) — 18 properties

## expenseReport

Browser definition `expenseReport`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | account |  |  | [`account`](account.md#account) |  |
| `accountingBookDetail` |  | expenseReport-accountingBookDetailCollection |  |  | [`expenseReport-accountingBookDetailCollection`](#expensereport-accountingbookdetailcollection) |  |
| `accountingapproval` | Accounting Approval | boolean |  |  |  |  |
| `acctcorpcardexp` |  | account |  |  | [`account`](account.md#account) |  |
| `advance` | Advance to Apply | number | double |  |  |  |
| `advance2` | Advance to Apply | number | double |  |  |  |
| `advanceaccount` |  | account |  |  | [`account`](account.md#account) |  |
| `amount` | Total Reimbursable Amount | number | double |  |  |  |
| `appliedRules` |  | expenseReport-appliedRulesCollection |  |  | [`expenseReport-appliedRulesCollection`](#expensereport-appliedrulescollection) |  |
| `approvalStatus` |  | object |  |  |  |  |
| `approvalStatus.id` | Internal identifier | string |  |  |  | `11`, `1`, `2`, `3` |
| `approvalStatus.refName` | Reference Name | string |  |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `complete` | Complete | boolean |  |  |  |  |
| `corporatecard` | Corporate Card | number | double |  |  |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReason` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReasonMemo` | Deletion Reason Memo | string |  |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `duedate` | Date Due | string | date |  |  |  |
| `entity` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `excludeFromGLNumbering` | Exclude from GL Audit Numbering | boolean |  |  |  |  |
| `expense` |  | expenseReport-expenseCollection |  |  | [`expenseReport-expenseCollection`](#expensereport-expensecollection) |  |
| `expensereportcurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `expensereportexchangerate` | Exchange Rate | number | double |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `lastModifiedDate` | Date Last Modified | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Purpose | string |  |  |  |  |
| `nextApprover` |  | employee |  |  | [`employee`](employee.md#employee) |  |
| `nexus` |  | nexus |  |  | [`nexus`](nexus.md#nexus) |  |
| `nonreimbursable` | Non-reimbursable Expenses (Tax Excl.) | number | double |  |  |  |
| `policyviolated` | Policy violated | boolean |  |  |  |  |
| `postingPeriod` |  | accountingPeriod |  |  | [`accountingPeriod`](accountingPeriod.md#accountingperiod) |  |
| `prevDate` | Previous Effective Date | string | date |  |  |  |
| `primaryBookBaseCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `reimbursable` | Reimbursable Expenses | number | double |  |  |  |
| `status` |  | object |  |  |  |  |
| `status.id` | Internal identifier | string |  |  |  | `A`, `B`, `C`, `D`, `E`, `V`, `F`, `G`, `H`, `I`, `J` |
| `status.refName` | Reference Name | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `subsidiaryTaxRegNum` | Subsidiary Tax Reg. Number | string |  |  |  |  |
| `supervisorapproval` | Supervisor Approval | boolean |  |  |  |  |
| `tax1Amt` | Tax | number | double |  |  |  |
| `tax2Amt` | PST | number | double |  |  |  |
| `taxDetails` |  | expenseReport-taxDetailsCollection |  |  | [`expenseReport-taxDetailsCollection`](#expensereport-taxdetailscollection) |  |
| `taxDetailsOverride` | Tax Details Override | boolean |  |  |  |  |
| `taxPointDate` | Tax Point Date | string | date |  |  |  |
| `taxPointDateOverride` | Tax Point Date Override | boolean |  |  |  |  |
| `taxRegOverride` | Tax Registration Override | boolean |  |  |  |  |
| `taxTotal` | Tax Total | number | double |  |  |  |
| `total` | Expenses Total | number | double |  |  |  |
| `totalbasecurrency` | Total in Base Currency | string |  |  |  |  |
| `tranDate` | Date | string | date |  |  |  |
| `tranId` | Exp. Rept. # | string |  |  |  |  |
| `transactionNumber` | Transaction Number | string |  |  |  |  |
| `usemulticurrency` | Use Multicurrency | boolean |  |  |  |  |
| `voided` | Voided | boolean |  |  |  |  |

## expenseReport-accountingBookDetailCollection

Browser definition `expenseReport-accountingBookDetailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | expenseReport-accountingBookDetailElement[] |  |  | [`expenseReport-accountingBookDetailElement`](#expensereport-accountingbookdetailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## expenseReport-accountingBookDetailElement

Browser definition `expenseReport-accountingBookDetailElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | accountingBook |  |  | [`accountingBook`](accountingBook.md#accountingbook) |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revRecOnRevCommitment` | Rev Rec on Rev Commit. | boolean |  |  |  |  |
| `tranIsVsoeBundle` | Transaction Is VSOE Bundle | boolean |  |  |  |  |

## expenseReport-appliedRulesCollection

Browser definition `expenseReport-appliedRulesCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | expenseReport-appliedRulesElement[] |  |  | [`expenseReport-appliedRulesElement`](#expensereport-appliedruleselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## expenseReport-appliedRulesElement

Browser definition `expenseReport-appliedRulesElement`.

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

## expenseReport-expenseCollection

Browser definition `expenseReport-expenseCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | expenseReport-expenseElement[] |  |  | [`expenseReport-expenseElement`](#expensereport-expenseelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## expenseReport-expenseElement

Browser definition `expenseReport-expenseElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amount` | Amount | number | double |  |  |  |
| `billingsubsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `category` |  | expenseCategory |  |  | [`expenseCategory`](expenseCategory.md#expensecategory) |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `corporatecreditcard` | Corporate Card | boolean |  |  |  |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `customer` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `exchangerate` | Exchange Rate | number | double |  |  |  |
| `expenseaccount` |  | account |  |  | [`account`](account.md#account) |  |
| `expensedate` | Date | string | date |  |  |  |
| `expmediaitem` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `foreignamount` | Foreign Amount | number | double |  |  |  |
| `grossAmt` | Gross Amt | number | double |  |  |  |
| `id` | ID | integer | int64 |  |  |  |
| `importedemployeeexpense` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `isBillable` | Billable | boolean |  |  |  |  |
| `isnonreimbursable` | Non-reimbursable | boolean |  |  |  |  |
| `line` | Line | string |  |  |  |  |
| `linked` |  | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `projecttask` |  | projectTask |  |  | [`projectTask`](projectTask.md#projecttask) |  |
| `quantity` | Quantity | number | float |  |  |  |
| `rate` | Rate | number | float |  |  |  |
| `raterequired` | Rate is Required | boolean |  |  |  |  |
| `receipt` | Receipt | boolean |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `refnumber` | Ref No. | integer | int64 |  |  |  |
| `tax1Amt` | Tax Amt | number | double |  |  |  |
| `taxAmount` | Tax Amount | number | double |  |  |  |
| `taxCode` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `taxDetailsReference` | Tax Details Reference | string |  |  |  |  |
| `taxRate1` | Tax Rate | number | double |  |  |  |
| `taxRate2` | PST | number | double |  |  |  |

## expenseReport-taxDetailsCollection

Browser definition `expenseReport-taxDetailsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | expenseReport-taxDetailsElement[] |  |  | [`expenseReport-taxDetailsElement`](#expensereport-taxdetailselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## expenseReport-taxDetailsElement

Browser definition `expenseReport-taxDetailsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `calcDetail` | Details | string |  |  |  |  |
| `lineName` | Name | string |  |  |  |  |
| `lineType` | Line type | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `netAmount` | Net Amount | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `taxAmount` | Tax Amount | number | double |  |  |  |
| `taxBasis` | Tax Basis | number | double |  |  |  |
| `taxCode` |  | salesTaxItem |  |  | [`salesTaxItem`](salesTaxItem.md#salestaxitem) |  |
| `taxDetailsReference` |  | object |  |  |  |  |
| `taxDetailsReference.id` | Internal identifier | string |  |  |  |  |
| `taxDetailsReference.refName` | Reference Name | string |  |  |  |  |
| `taxRate` | Tax Rate | number | double |  |  |  |
| `taxType` | Tax Type | string |  |  |  |  |

## expenseReportCollection

Browser definition `expenseReportCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | expenseReport[] |  |  | [`expenseReport`](#expensereport) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## expenseReportSelectOptions

Browser definition `expenseReportSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `acctcorpcardexp` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `advanceaccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `approvalStatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deletionReason` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `entity` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `expensereportcurrency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `nextApprover` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `nexus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `postingPeriod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `primaryBookBaseCurrency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `status` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiaryTaxRegNum` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
