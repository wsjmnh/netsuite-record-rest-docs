# Schemas: budgetimport

Property tables for definitions owned by `budgetimport`.

Record page: [budgetimport](../records/budgetimport.md).

## Index

- [budgetimport](#budgetimport) — 43 properties
- [budgetimportCollection](#budgetimportcollection) — 6 properties
- [budgetimportSelectOptions](#budgetimportselectoptions) — 11 properties

## budgetimport

Browser definition `budgetimport`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | account |  |  | [`account`](account.md#account) |  |
| `accountingBook` |  | accountingBook |  |  | [`accountingBook`](accountingBook.md#accountingbook) |  |
| `amount` | Amount | number | double |  |  |  |
| `budgetType` | Global | boolean |  |  |  |  |
| `category` |  | budgetCategory |  |  | [`budgetCategory`](budgetCategory.md#budgetcategory) |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `currencyPrecision` |  | string |  |  |  |  |
| `customer` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `item` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `periodAmount1` | Period {1} Amount | number | double |  |  |  |
| `periodAmount10` | Period {1} Amount | number | double |  |  |  |
| `periodAmount11` | Period {1} Amount | number | double |  |  |  |
| `periodAmount12` | Period {1} Amount | number | double |  |  |  |
| `periodAmount13` | Period {1} Amount | number | double |  |  |  |
| `periodAmount14` | Period {1} Amount | number | double |  |  |  |
| `periodAmount15` | Period {1} Amount | number | double |  |  |  |
| `periodAmount16` | Period {1} Amount | number | double |  |  |  |
| `periodAmount17` | Period {1} Amount | number | double |  |  |  |
| `periodAmount18` | Period {1} Amount | number | double |  |  |  |
| `periodAmount19` | Period {1} Amount | number | double |  |  |  |
| `periodAmount2` | Period {1} Amount | number | double |  |  |  |
| `periodAmount20` | Period {1} Amount | number | double |  |  |  |
| `periodAmount21` | Period {1} Amount | number | double |  |  |  |
| `periodAmount22` | Period {1} Amount | number | double |  |  |  |
| `periodAmount23` | Period {1} Amount | number | double |  |  |  |
| `periodAmount24` | Period {1} Amount | number | double |  |  |  |
| `periodAmount3` | Period {1} Amount | number | double |  |  |  |
| `periodAmount4` | Period {1} Amount | number | double |  |  |  |
| `periodAmount5` | Period {1} Amount | number | double |  |  |  |
| `periodAmount6` | Period {1} Amount | number | double |  |  |  |
| `periodAmount7` | Period {1} Amount | number | double |  |  |  |
| `periodAmount8` | Period {1} Amount | number | double |  |  |  |
| `periodAmount9` | Period {1} Amount | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `year` |  | accountingPeriod |  |  | [`accountingPeriod`](accountingPeriod.md#accountingperiod) |  |
| `yearNoAccountingPeriod` | Year | string |  |  |  |  |

## budgetimportCollection

Browser definition `budgetimportCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | budgetimport[] |  |  | [`budgetimport`](#budgetimport) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## budgetimportSelectOptions

Browser definition `budgetimportSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `accountingBook` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `category` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `currency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customer` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `item` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `year` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
