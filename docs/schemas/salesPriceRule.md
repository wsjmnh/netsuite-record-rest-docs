# Schemas: salesPriceRule

Property tables for definitions owned by `salesPriceRule`.

Record page: [salesPriceRule](../records/salesPriceRule.md).

## Index

- [salesPriceRule](#salespricerule) — 15 properties
- [salesPriceRule-customerDimensionCollection](#salespricerule-customerdimensioncollection) — 6 properties
- [salesPriceRule-customerDimensionElement](#salespricerule-customerdimensionelement) — 6 properties
- [salesPriceRule-customerGroupsCollection](#salespricerule-customergroupscollection) — 6 properties
- [salesPriceRule-customerGroupsElement](#salespricerule-customergroupselement) — 6 properties
- [salesPriceRuleCollection](#salespricerulecollection) — 6 properties
- [salesPriceRuleSelectOptions](#salespriceruleselectoptions) — 1 properties

## salesPriceRule

Browser definition `salesPriceRule`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customerDimension` |  | salesPriceRule-customerDimensionCollection |  |  | [`salesPriceRule-customerDimensionCollection`](#salespricerule-customerdimensioncollection) |  |
| `customerGroups` |  | salesPriceRule-customerGroupsCollection |  |  | [`salesPriceRule-customerGroupsCollection`](#salespricerule-customergroupscollection) |  |
| `dateCreated` | Date Created | string | date-time |  |  |  |
| `description` | Description | string |  |  |  |  |
| `endDate` | End Date | string | date |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isAppliedToAllItems` | Apply to All Items | boolean |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Name | string |  |  |  |  |
| `priceLevel` |  | priceLevel |  |  | [`priceLevel`](priceLevel.md#pricelevel) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `startDate` | Start Date | string | date |  |  |  |

## salesPriceRule-customerDimensionCollection

Browser definition `salesPriceRule-customerDimensionCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | salesPriceRule-customerDimensionElement[] |  |  | [`salesPriceRule-customerDimensionElement`](#salespricerule-customerdimensionelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## salesPriceRule-customerDimensionElement

Browser definition `salesPriceRule-customerDimensionElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `Id` | Internal ID | integer | int64 |  |  |  |
| `customer` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `dateCreated` | Date Created | string | date-time |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## salesPriceRule-customerGroupsCollection

Browser definition `salesPriceRule-customerGroupsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | salesPriceRule-customerGroupsElement[] |  |  | [`salesPriceRule-customerGroupsElement`](#salespricerule-customergroupselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## salesPriceRule-customerGroupsElement

Browser definition `salesPriceRule-customerGroupsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `Id` | Internal ID | integer | int64 |  |  |  |
| `customerGroup` |  | entityGroup |  |  | [`entityGroup`](entityGroup.md#entitygroup) |  |
| `dateCreated` | Date Created | string | date-time |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## salesPriceRuleCollection

Browser definition `salesPriceRuleCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | salesPriceRule[] |  |  | [`salesPriceRule`](#salespricerule) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## salesPriceRuleSelectOptions

Browser definition `salesPriceRuleSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `priceLevel` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
