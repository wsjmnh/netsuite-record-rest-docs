# Schemas: priceLevel

Property tables for definitions owned by `priceLevel`.

Record page: [priceLevel](../records/priceLevel.md).

## Index

- [priceLevel](#pricelevel) — 15 properties
- [priceLevelCollection](#pricelevelcollection) — 6 properties

## priceLevel

Browser definition `priceLevel`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `discountPct` | Markup/Discount % | number | double |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `isOnline` | Online Price Level | boolean |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `longitemtype` |  | string |  |  |  |  |
| `name` | Price Level | string |  |  |  |  |
| `priceCalculationFormula` | Price Calculation Formula | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `tname` |  | string |  |  |  |  |
| `updateExistingPrices` | Update Prices for Items Using This Price Level | boolean |  |  |  |  |
| `updateExistingTaxExclusivePrices` | Update Tax Exclusive Prices | boolean |  |  |  |  |
| `updateExistingTaxInclusivePrices` | Update Tax Inclusive Prices | boolean |  |  |  |  |

## priceLevelCollection

Browser definition `priceLevelCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | priceLevel[] |  |  | [`priceLevel`](#pricelevel) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |
