# Schemas: inventoryCostRevaluation

Property tables for definitions owned by `inventoryCostRevaluation`.

Record page: [inventoryCostRevaluation](../records/inventoryCostRevaluation.md).

## Index

- [inventoryCostRevaluation](#inventorycostrevaluation) — 34 properties
- [inventoryCostRevaluation-accountingBookDetailCollection](#inventorycostrevaluation-accountingbookdetailcollection) — 6 properties
- [inventoryCostRevaluation-accountingBookDetailElement](#inventorycostrevaluation-accountingbookdetailelement) — 7 properties
- [inventoryCostRevaluation-costComponentCollection](#inventorycostrevaluation-costcomponentcollection) — 6 properties
- [inventoryCostRevaluation-costComponentElement](#inventorycostrevaluation-costcomponentelement) — 14 properties
- [inventoryCostRevaluationCollection](#inventorycostrevaluationcollection) — 6 properties
- [inventoryCostRevaluationSelectOptions](#inventorycostrevaluationselectoptions) — 10 properties

## inventoryCostRevaluation

Browser definition `inventoryCostRevaluation`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | account |  |  | [`account`](account.md#account) |  |
| `accountingBookDetail` |  | inventoryCostRevaluation-accountingBookDetailCollection |  |  | [`inventoryCostRevaluation-accountingBookDetailCollection`](#inventorycostrevaluation-accountingbookdetailcollection) |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `costComponent` |  | inventoryCostRevaluation-costComponentCollection |  |  | [`inventoryCostRevaluation-costComponentCollection`](#inventorycostrevaluation-costcomponentcollection) |  |
| `costingMethod` | Costing Method | string |  |  |  |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReason` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReasonMemo` | Deletion Reason Memo | string |  |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `excludeFromGLNumbering` | Exclude from GL Audit Numbering | boolean |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `inventoryValue` | New Inventory Value | number | double |  |  |  |
| `ispurchase` |  | string |  |  |  |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemCostCategory` | Item Cost Category | integer | int64 |  |  |  |
| `itemType` | Item Type | string |  |  |  |  |
| `lastModifiedDate` | Date Last Modified | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `overheadType` | Overhead Type | string |  |  |  |  |
| `postingPeriod` |  | accountingPeriod |  |  | [`accountingPeriod`](accountingPeriod.md#accountingperiod) |  |
| `prevDate` | Previous Effective Date | string | date |  |  |  |
| `primaryBookBaseCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `selloutLineAmount` | Sellout Line Amount | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `total` | Adjustment Amount | number | double |  |  |  |
| `tranDate` | Date | string | date |  |  |  |
| `tranId` | Ref No. | string |  |  |  |  |
| `transactionNumber` | Transaction Number | string |  |  |  |  |
| `unitCost` | New Unit Cost | number | double |  |  |  |

## inventoryCostRevaluation-accountingBookDetailCollection

Browser definition `inventoryCostRevaluation-accountingBookDetailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | inventoryCostRevaluation-accountingBookDetailElement[] |  |  | [`inventoryCostRevaluation-accountingBookDetailElement`](#inventorycostrevaluation-accountingbookdetailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## inventoryCostRevaluation-accountingBookDetailElement

Browser definition `inventoryCostRevaluation-accountingBookDetailElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | accountingBook |  |  | [`accountingBook`](accountingBook.md#accountingbook) |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revRecOnRevCommitment` | Rev Rec on Rev Commit. | boolean |  |  |  |  |
| `tranIsVsoeBundle` | Transaction Is VSOE Bundle | boolean |  |  |  |  |

## inventoryCostRevaluation-costComponentCollection

Browser definition `inventoryCostRevaluation-costComponentCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | inventoryCostRevaluation-costComponentElement[] |  |  | [`inventoryCostRevaluation-costComponentElement`](#inventorycostrevaluation-costcomponentelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## inventoryCostRevaluation-costComponentElement

Browser definition `inventoryCostRevaluation-costComponentElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amount` | Amount | string |  |  |  |  |
| `componentItem` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `conversionRate` | Conversion Rate {1} | number | float |  |  |  |
| `cost` | Cost | number | double |  |  |  |
| `costCategory` |  | costCategory |  |  | [`costCategory`](costCategory.md#costcategory) |  |
| `costType` | Cost Category | string |  |  |  |  |
| `isMaterialOverhead` | Is Material Overhead | string |  |  |  |  |
| `isRouting` | Is Routing | string |  |  |  |  |
| `lineId` | Line Id | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `overheadType` | Overhead Type | string |  |  |  |  |
| `quantity` | Quantity | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `units` | Units | string |  |  |  |  |

## inventoryCostRevaluationCollection

Browser definition `inventoryCostRevaluationCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | inventoryCostRevaluation[] |  |  | [`inventoryCostRevaluation`](#inventorycostrevaluation) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## inventoryCostRevaluationSelectOptions

Browser definition `inventoryCostRevaluationSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deletionReason` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `item` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `postingPeriod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `primaryBookBaseCurrency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
