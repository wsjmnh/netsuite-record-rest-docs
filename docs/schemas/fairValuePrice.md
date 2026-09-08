# Schemas: fairValuePrice

Property tables for definitions owned by `fairValuePrice`.

Record page: [fairValuePrice](../records/fairValuePrice.md).

## Index

- [fairValuePrice](#fairvalueprice) — 28 properties
- [fairValuePriceCollection](#fairvaluepricecollection) — 6 properties
- [fairValuePriceSelectOptions](#fairvaluepriceselectoptions) — 12 properties

## fairValuePrice

Browser definition `fairValuePrice`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | accountingBook |  |  | [`accountingBook`](accountingBook.md#accountingbook) |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `customer` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `endDate` | End Date | string | date |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `fairValue` | Base Fair Value | number | float |  |  |  |
| `fairValueFormula` |  | fairValueFormula |  |  | [`fairValueFormula`](fairValueFormula.md#fairvalueformula) |  |
| `fairValueRangePolicy` |  | object |  |  |  |  |
| `fairValueRangePolicy.id` | Internal identifier | string |  |  |  | `HIGH`, `LOW`, `BOUNDARY`, `FAIRVALUE` |
| `fairValueRangePolicy.refName` | Reference Name | string |  |  |  |  |
| `highValue` | High Value | number | float |  |  |  |
| `highValuePercent` | High Value Percent | number | double |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isVsoePrice` | Is VSOE Price? | boolean |  |  |  |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemRevenueCategory` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `lowValue` | Low Value | number | float |  |  |  |
| `lowValuePercent` | Low Value Percent | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `sourceType` |  | object |  |  |  |  |
| `sourceType.id` | Internal identifier | string |  |  |  | `SUBSCRIPTION_LINE`, `TRANSACTION_LINE`, `PROJECT_REVENUE_RULE`, `THIRD_PARTY` |
| `sourceType.refName` | Reference Name | string |  |  |  |  |
| `startDate` | Start Date | string | date |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `units` | Units | string |  |  |  |  |
| `unitsType` |  | unitsType |  |  | [`unitsType`](unitsType.md#unitstype) |  |

## fairValuePriceCollection

Browser definition `fairValuePriceCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | fairValuePrice[] |  |  | [`fairValuePrice`](#fairvalueprice) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## fairValuePriceSelectOptions

Browser definition `fairValuePriceSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `currency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customer` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `fairValueFormula` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `fairValueRangePolicy` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `item` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `itemRevenueCategory` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `sourceType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `units` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `unitsType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
