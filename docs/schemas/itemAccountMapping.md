# Schemas: itemAccountMapping

Property tables for definitions owned by `itemAccountMapping`.

Record page: [itemAccountMapping](../records/itemAccountMapping.md).

## Index

- [itemAccountMapping](#itemaccountmapping) — 23 properties
- [itemAccountMappingCollection](#itemaccountmappingcollection) — 6 properties
- [itemAccountMappingSelectOptions](#itemaccountmappingselectoptions) — 9 properties

## itemAccountMapping

Browser definition `itemAccountMapping`.

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
| `itemAccount` |  | object |  |  |  |  |
| `itemAccount.id` | Internal identifier | string |  |  |  | `CUSTOMERRETURNVARIANCE`, `SCRAP`, `PAYMENT`, `ACCOUNTSRECEIVABLE`, `VENDORBILLQUANTITYVARIANCE`, `FXADJUSTMENTREVENUE`, `COGS`, `UNBUILDVARIANCE`, `PRODUCTIONQUANTITYVARIANCE`, `INTERCOCOGS`, `INTERCODEFERREDREVENUE`, `GAINLOSS`, `PRODUCTIONPRICEVARIANCE`, `PURCHASEPRICEVARIANCE`, `INCOME`, `DEFERREDREVENUE`, `INTERCOEXPENSE`, `DROPSHIPEXPENSE`, `WIPVARIANCE`, `DEFERREDREVENUERECLASS`, `WRITEOFF`, `INTERCOINCOME`, `DEFERRAL`, `LIABILITY`, `ASSET`, `VENDORRETURNVARIANCE`, `DISCOUNT`, `VENDORCONSIGNED`, `VENDORBILLPRICEVARIANCE`, `VENDORBILLEXCHRATEVARIANCE`, `MARKUP`, `EXPENSE`, `ACCOUNTSPAYABLE`, `WIP` |
| `itemAccount.refName` | Reference Name | string |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `locationDisplayValue` | Location | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `sourceAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |

## itemAccountMappingCollection

Browser definition `itemAccountMappingCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | itemAccountMapping[] |  |  | [`itemAccountMapping`](#itemaccountmapping) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## itemAccountMappingSelectOptions

Browser definition `itemAccountMappingSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `destinationAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `itemAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `sourceAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
