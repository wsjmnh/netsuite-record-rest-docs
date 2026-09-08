# Schemas: statisticalJournalEntry

Property tables for definitions owned by `statisticalJournalEntry`.

Record page: [statisticalJournalEntry](../records/statisticalJournalEntry.md).

## Index

- [statisticalJournalEntry](#statisticaljournalentry) — 38 properties
- [statisticalJournalEntry-lineCollection](#statisticaljournalentry-linecollection) — 6 properties
- [statisticalJournalEntry-lineElement](#statisticaljournalentry-lineelement) — 16 properties
- [statisticalJournalEntryCollection](#statisticaljournalentrycollection) — 6 properties
- [statisticalJournalEntrySelectOptions](#statisticaljournalentryselectoptions) — 15 properties

## statisticalJournalEntry

Browser definition `statisticalJournalEntry`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `absoluteUpdate` | Absolute Update | boolean |  |  |  |  |
| `absoluteUpdateJournalLink` |  | statisticalJournalEntry |  |  | [`statisticalJournalEntry`](#statisticaljournalentry) |  |
| `approvalStatus` |  | object |  |  |  |  |
| `approvalStatus.id` | Internal identifier | string |  |  |  | `11`, `1`, `2`, `3` |
| `approvalStatus.refName` | Reference Name | string |  |  |  |  |
| `approved` | Approved | boolean |  |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReason` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReasonMemo` | Deletion Reason Memo | string |  |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `excludeFromGLNumbering` | Exclude from GL Audit Numbering | boolean |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isReversal` | Is Reversal | boolean |  |  |  |  |
| `lastModifiedDate` | Date Last Modified | string | date-time |  |  |  |
| `line` |  | statisticalJournalEntry-lineCollection |  |  | [`statisticalJournalEntry-lineCollection`](#statisticaljournalentry-linecollection) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `nextApprover` |  | employee |  |  | [`employee`](employee.md#employee) |  |
| `offsetJournalLink` |  | statisticalJournalEntry |  |  | [`statisticalJournalEntry`](#statisticaljournalentry) |  |
| `parentStat` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `postingPeriod` |  | accountingPeriod |  |  | [`accountingPeriod`](accountingPeriod.md#accountingperiod) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `reversal` |  | statisticalJournalEntry |  |  | [`statisticalJournalEntry`](#statisticaljournalentry) |  |
| `reversalDate` | Reversal Date | string | date |  |  |  |
| `reversalDefer` | Defer Entry | boolean |  |  |  |  |
| `reversalEntry` | Reversal No. | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `total` | Total | string |  |  |  |  |
| `tranDate` | Date | string | date |  |  |  |
| `tranId` | Entry No. | string |  |  |  |  |
| `transactionNumber` | Transaction Number | string |  |  |  |  |
| `unit` | Unit of Measure | string |  |  |  |  |
| `unitsType` |  | unitsType |  |  | [`unitsType`](unitsType.md#unitstype) |  |
| `void` | Void | boolean |  |  |  |  |

## statisticalJournalEntry-lineCollection

Browser definition `statisticalJournalEntry-lineCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | statisticalJournalEntry-lineElement[] |  |  | [`statisticalJournalEntry-lineElement`](#statisticaljournalentry-lineelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## statisticalJournalEntry-lineElement

Browser definition `statisticalJournalEntry-lineElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | account |  |  | [`account`](account.md#account) |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `debit` | Amount | number | double |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `eliminate` | Eliminate | boolean |  |  |  |  |
| `entity` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `line` | Line Id | integer | int64 |  |  |  |
| `lineCreatedDate` | Line Created Date | string | date-time |  |  |  |
| `lineLastModifiedDate` | Line Last Modified Date | string | date-time |  |  |  |
| `lineUnit` | Units | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `previewDebit` | Amount (Base Unit) | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revenueRecognitionRule` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |

## statisticalJournalEntryCollection

Browser definition `statisticalJournalEntryCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | statisticalJournalEntry[] |  |  | [`statisticalJournalEntry`](#statisticaljournalentry) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## statisticalJournalEntrySelectOptions

Browser definition `statisticalJournalEntrySelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `absoluteUpdateJournalLink` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `approvalStatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deletionReason` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `nextApprover` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `offsetJournalLink` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `parentStat` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `postingPeriod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `reversal` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `unit` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `unitsType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
