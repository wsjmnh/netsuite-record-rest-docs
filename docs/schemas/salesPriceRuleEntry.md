# Schemas: salesPriceRuleEntry

Property tables for definitions owned by `salesPriceRuleEntry`.

Record page: [salesPriceRuleEntry](../records/salesPriceRuleEntry.md).

## Index

- [salesPriceRuleEntry](#salespriceruleentry) — 8 properties
- [salesPriceRuleEntryCollection](#salespriceruleentrycollection) — 6 properties
- [salesPriceRuleEntrySelectOptions](#salespriceruleentryselectoptions) — 2 properties

## salesPriceRuleEntry

Browser definition `salesPriceRuleEntry`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `dateCreated` | Date Created | string | date-time |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `priceRule` |  | salesPriceRule |  |  | [`salesPriceRule`](salesPriceRule.md#salespricerule) |  |
| `refName` | Reference Name | string |  |  |  |  |

## salesPriceRuleEntryCollection

Browser definition `salesPriceRuleEntryCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | salesPriceRuleEntry[] |  |  | [`salesPriceRuleEntry`](#salespriceruleentry) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## salesPriceRuleEntrySelectOptions

Browser definition `salesPriceRuleEntrySelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `item` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `priceRule` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
