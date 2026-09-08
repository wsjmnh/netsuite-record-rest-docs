# Schemas: competitor

Property tables for definitions owned by `competitor`.

Record page: [competitor](../records/competitor.md).

## Index

- [competitor](#competitor) — 14 properties
- [competitorCollection](#competitorcollection) — 6 properties
- [competitorSelectOptions](#competitorselectoptions) — 1 properties

## competitor

Browser definition `competitor`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `description` | Description | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Name | string |  |  |  |  |
| `productService` | Products/Services | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `strategy` | Strategy | string |  |  |  |  |
| `strengths` | Strengths | string |  |  |  |  |
| `url` | Web Address | string |  |  |  |  |
| `weaknesses` | Weaknesses | string |  |  |  |  |

## competitorCollection

Browser definition `competitorCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | competitor[] |  |  | [`competitor`](#competitor) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## competitorSelectOptions

Browser definition `competitorSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
