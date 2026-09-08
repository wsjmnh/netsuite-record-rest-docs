# Schemas: globalAccountMapping

Property tables for definitions owned by `globalAccountMapping`.

Record page: [globalAccountMapping](../records/globalAccountMapping.md).

## Index

- [globalAccountMapping](#globalaccountmapping) — 20 properties
- [globalAccountMappingCollection](#globalaccountmappingcollection) — 6 properties
- [globalAccountMappingSelectOptions](#globalaccountmappingselectoptions) — 8 properties

## globalAccountMapping

Browser definition `globalAccountMapping`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | accountingBook |  |  | [`accountingBook`](accountingBook.md#accountingbook) |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `classDisplayValue` | Class | string |  |  |  |  |
| `customField` | Custom Field | string |  |  |  |  |
| `customFieldCompId` | Custom Field CompId | string |  |  |  |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `departmentDisplayValue` | Department | string |  |  |  |  |
| `destinationAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `effectiveDate` | Effective Date | string | date |  |  |  |
| `endDate` | End Date | string | date |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `locationDisplayValue` | Location | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `sourceAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |

## globalAccountMappingCollection

Browser definition `globalAccountMappingCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | globalAccountMapping[] |  |  | [`globalAccountMapping`](#globalaccountmapping) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## globalAccountMappingSelectOptions

Browser definition `globalAccountMappingSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `destinationAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `sourceAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
