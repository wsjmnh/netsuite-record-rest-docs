# Schemas: periodEndJournal

Property tables for definitions owned by `periodEndJournal`.

Record page: [periodEndJournal](../records/periodEndJournal.md).

## Index

- [periodEndJournal](#periodendjournal) — 33 properties
- [periodEndJournal-lineCollection](#periodendjournal-linecollection) — 6 properties
- [periodEndJournal-lineElement](#periodendjournal-lineelement) — 8 properties
- [periodEndJournalCollection](#periodendjournalcollection) — 6 properties
- [periodEndJournalSelectOptions](#periodendjournalselectoptions) — 13 properties

## periodEndJournal

Browser definition `periodEndJournal`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | accountingBook |  |  | [`accountingBook`](accountingBook.md#accountingbook) |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `creditTotal` | Credit | number | double |  |  |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `debitTotal` | Debit | number | double |  |  |  |
| `deletionReason` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReasonMemo` | Deletion Reason Memo | string |  |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `excludeFromGLNumbering` | Exclude from GL Audit Numbering | boolean |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isReversal` | Is Reversal | boolean |  |  |  |  |
| `lastModifiedDate` | Date Last Modified | string | date-time |  |  |  |
| `line` |  | periodEndJournal-lineCollection |  |  | [`periodEndJournal-lineCollection`](#periodendjournal-linecollection) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `mainAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `memo` | Memo | string |  |  |  |  |
| `pairedPEJE` |  | periodEndJournal |  |  | [`periodEndJournal`](#periodendjournal) |  |
| `pejeType` | Type | string |  |  |  |  |
| `postingPeriod` |  | accountingPeriod |  |  | [`accountingPeriod`](accountingPeriod.md#accountingperiod) |  |
| `prevDate` | Previous Effective Date | string | date |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `sourceSubsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `status` |  | object |  |  |  |  |
| `status.id` | Internal identifier | string |  |  |  | `A`, `R`, `B`, `Y` |
| `status.refName` | Reference Name | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `tranDate` | Date | string | date |  |  |  |
| `tranId` | Entry No. | string |  |  |  |  |
| `transactionNumber` | Transaction Number | string |  |  |  |  |

## periodEndJournal-lineCollection

Browser definition `periodEndJournal-lineCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | periodEndJournal-lineElement[] |  |  | [`periodEndJournal-lineElement`](#periodendjournal-lineelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## periodEndJournal-lineElement

Browser definition `periodEndJournal-lineElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | account |  |  | [`account`](account.md#account) |  |
| `credit` | Credit | number | double |  |  |  |
| `debit` | Debit | number | double |  |  |  |
| `detailType` | Detail Type | string |  |  |  |  |
| `line` | Period End Journal Line | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `memo` | Memo | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## periodEndJournalCollection

Browser definition `periodEndJournalCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | periodEndJournal[] |  |  | [`periodEndJournal`](#periodendjournal) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## periodEndJournalSelectOptions

Browser definition `periodEndJournalSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `currency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deletionReason` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `mainAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `pairedPEJE` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `postingPeriod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `sourceSubsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `status` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
