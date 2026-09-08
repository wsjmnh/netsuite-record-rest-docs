# Schemas: couponCode

Property tables for definitions owned by `couponCode`.

Record page: [couponCode](../records/couponCode.md).

## Index

- [couponCode](#couponcode) — 10 properties
- [couponCodeCollection](#couponcodecollection) — 6 properties
- [couponCodeSelectOptions](#couponcodeselectoptions) — 2 properties

## couponCode

Browser definition `couponCode`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `code` | Code | string |  |  |  |  |
| `dateSent` | Date Sent | string | date |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `promotion` |  | promotionCode |  |  | [`promotionCode`](promotionCode.md#promotioncode) |  |
| `recipient` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `useCount` | Used Count | string |  |  |  |  |
| `used` | Used | boolean |  |  |  |  |

## couponCodeCollection

Browser definition `couponCodeCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | couponCode[] |  |  | [`couponCode`](#couponcode) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## couponCodeSelectOptions

Browser definition `couponCodeSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `promotion` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `recipient` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
