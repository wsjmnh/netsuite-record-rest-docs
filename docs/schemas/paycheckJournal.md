# Schemas: paycheckJournal

Property tables for definitions owned by `paycheckJournal`.

Record page: [paycheckJournal](../records/paycheckJournal.md).

## Index

- [paycheckJournal](#paycheckjournal) — 30 properties
- [paycheckJournal-companycontributionCollection](#paycheckjournal-companycontributioncollection) — 6 properties
- [paycheckJournal-companycontributionElement](#paycheckjournal-companycontributionelement) — 8 properties
- [paycheckJournal-companytaxCollection](#paycheckjournal-companytaxcollection) — 6 properties
- [paycheckJournal-companytaxElement](#paycheckjournal-companytaxelement) — 8 properties
- [paycheckJournal-deductionCollection](#paycheckjournal-deductioncollection) — 6 properties
- [paycheckJournal-deductionElement](#paycheckjournal-deductionelement) — 8 properties
- [paycheckJournal-earningCollection](#paycheckjournal-earningcollection) — 6 properties
- [paycheckJournal-earningElement](#paycheckjournal-earningelement) — 9 properties
- [paycheckJournal-employeetaxCollection](#paycheckjournal-employeetaxcollection) — 6 properties
- [paycheckJournal-employeetaxElement](#paycheckjournal-employeetaxelement) — 8 properties
- [paycheckJournalCollection](#paycheckjournalcollection) — 6 properties
- [paycheckJournalSelectOptions](#paycheckjournalselectoptions) — 11 properties

## paycheckJournal

Browser definition `paycheckJournal`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | account |  |  | [`account`](account.md#account) |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `companycontribution` |  | paycheckJournal-companycontributionCollection |  |  | [`paycheckJournal-companycontributionCollection`](#paycheckjournal-companycontributioncollection) |  |
| `companytax` |  | paycheckJournal-companytaxCollection |  |  | [`paycheckJournal-companytaxCollection`](#paycheckjournal-companytaxcollection) |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deduction` |  | paycheckJournal-deductionCollection |  |  | [`paycheckJournal-deductionCollection`](#paycheckjournal-deductioncollection) |  |
| `deletionReason` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReasonMemo` | Deletion Reason Memo | string |  |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `earning` |  | paycheckJournal-earningCollection |  |  | [`paycheckJournal-earningCollection`](#paycheckjournal-earningcollection) |  |
| `employee` |  | employee |  |  | [`employee`](employee.md#employee) |  |
| `employeetax` |  | paycheckJournal-employeetaxCollection |  |  | [`paycheckJournal-employeetaxCollection`](#paycheckjournal-employeetaxcollection) |  |
| `exchangerate` | Exchange Rate | number | float |  |  |  |
| `excludeFromGLNumbering` | Exclude from GL Audit Numbering | boolean |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `lastModifiedDate` | Date Last Modified | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `postingPeriod` |  | accountingPeriod |  |  | [`accountingPeriod`](accountingPeriod.md#accountingperiod) |  |
| `prevDate` | Previous Effective Date | string | date |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `taxPeriod` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `tranDate` | Date | string | date |  |  |  |
| `tranId` | Entry No. | string |  |  |  |  |
| `transactionNumber` | Transaction Number | string |  |  |  |  |
| `voided` | Voided | boolean |  |  |  |  |

## paycheckJournal-companycontributionCollection

Browser definition `paycheckJournal-companycontributionCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | paycheckJournal-companycontributionElement[] |  |  | [`paycheckJournal-companycontributionElement`](#paycheckjournal-companycontributionelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## paycheckJournal-companycontributionElement

Browser definition `paycheckJournal-companycontributionElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amount` | Amount | number | double |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `id` | Line Id | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `payrollItem` |  | payrollItem |  |  | [`payrollItem`](payrollItem.md#payrollitem) |  |
| `refName` | Reference Name | string |  |  |  |  |

## paycheckJournal-companytaxCollection

Browser definition `paycheckJournal-companytaxCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | paycheckJournal-companytaxElement[] |  |  | [`paycheckJournal-companytaxElement`](#paycheckjournal-companytaxelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## paycheckJournal-companytaxElement

Browser definition `paycheckJournal-companytaxElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amount` | Amount | number | double |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `id` | Line Id | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `payrollItem` |  | payrollItem |  |  | [`payrollItem`](payrollItem.md#payrollitem) |  |
| `refName` | Reference Name | string |  |  |  |  |

## paycheckJournal-deductionCollection

Browser definition `paycheckJournal-deductionCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | paycheckJournal-deductionElement[] |  |  | [`paycheckJournal-deductionElement`](#paycheckjournal-deductionelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## paycheckJournal-deductionElement

Browser definition `paycheckJournal-deductionElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amount` | Amount | number | double |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `id` | Line Id | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `payrollItem` |  | payrollItem |  |  | [`payrollItem`](payrollItem.md#payrollitem) |  |
| `refName` | Reference Name | string |  |  |  |  |

## paycheckJournal-earningCollection

Browser definition `paycheckJournal-earningCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | paycheckJournal-earningElement[] |  |  | [`paycheckJournal-earningElement`](#paycheckjournal-earningelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## paycheckJournal-earningElement

Browser definition `paycheckJournal-earningElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amount` | Amount | number | double |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `hours` | Hours | number | float |  |  |  |
| `id` | Line Id | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `payrollItem` |  | payrollItem |  |  | [`payrollItem`](payrollItem.md#payrollitem) |  |
| `refName` | Reference Name | string |  |  |  |  |

## paycheckJournal-employeetaxCollection

Browser definition `paycheckJournal-employeetaxCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | paycheckJournal-employeetaxElement[] |  |  | [`paycheckJournal-employeetaxElement`](#paycheckjournal-employeetaxelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## paycheckJournal-employeetaxElement

Browser definition `paycheckJournal-employeetaxElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amount` | Amount | number | double |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `id` | Line Id | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `payrollItem` |  | payrollItem |  |  | [`payrollItem`](payrollItem.md#payrollitem) |  |
| `refName` | Reference Name | string |  |  |  |  |

## paycheckJournalCollection

Browser definition `paycheckJournalCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | paycheckJournal[] |  |  | [`paycheckJournal`](#paycheckjournal) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## paycheckJournalSelectOptions

Browser definition `paycheckJournalSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `currency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deletionReason` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `employee` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `postingPeriod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `taxPeriod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
