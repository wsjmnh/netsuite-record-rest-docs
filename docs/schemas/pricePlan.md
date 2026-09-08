# Schemas: pricePlan

Property tables for definitions owned by `pricePlan`.

Record page: [pricePlan](../records/pricePlan.md).

## Index

- [pricePlan](#priceplan) — 14 properties
- [pricePlan-priceTiersCollection](#priceplan-pricetierscollection) — 6 properties
- [pricePlan-priceTiersElement](#priceplan-pricetierselement) — 10 properties
- [pricePlanCollection](#priceplancollection) — 6 properties
- [pricePlanSelectOptions](#priceplanselectoptions) — 3 properties

## pricePlan

Browser definition `pricePlan`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `maximumAmount` | Maximum Amount | number | double |  |  |  |
| `minimumAmount` | Minimum Amount | number | double |  |  |  |
| `prepayAmount` | Prepay Amount | number | double |  |  |  |
| `prepayMinBalance` | Prepay Minimum Balance | number | double |  |  |  |
| `pricePlanType` |  | object |  |  |  |  |
| `pricePlanType.id` | Internal identifier | string |  |  |  | `1`, `2`, `3`, `4`, `5` |
| `pricePlanType.refName` | Reference Name | string |  |  |  |  |
| `priceTiers` |  | pricePlan-priceTiersCollection |  |  | [`pricePlan-priceTiersCollection`](#priceplan-pricetierscollection) |  |
| `refName` | Reference Name | string |  |  |  |  |

## pricePlan-priceTiersCollection

Browser definition `pricePlan-priceTiersCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | pricePlan-priceTiersElement[] |  |  | [`pricePlan-priceTiersElement`](#priceplan-pricetierselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## pricePlan-priceTiersElement

Browser definition `pricePlan-priceTiersElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `fromVal` | From Quantity | integer | int64 |  |  |  |
| `internalId` | Internal ID | integer | int64 |  |  |  |
| `lineId` | Line Id | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `maxAmount` | Maximum Amount | number | double |  |  |  |
| `minAmount` | Minimum Amount | number | double |  |  |  |
| `priceTier` | Tiers | string |  |  |  |  |
| `pricingOption` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `value` | Value | number | double |  |  |  |

## pricePlanCollection

Browser definition `pricePlanCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | pricePlan[] |  |  | [`pricePlan`](#priceplan) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## pricePlanSelectOptions

Browser definition `pricePlanSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `currency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `pricePlanType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
