# Schemas: pricingGroup

Property tables for definitions owned by `pricingGroup`.

Record page: [pricingGroup](../records/pricingGroup.md).

## Index

- [pricingGroup](#pricinggroup) — 9 properties
- [pricingGroupCollection](#pricinggroupcollection) — 6 properties

## pricingGroup

Browser definition `pricingGroup`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `longitemtype` |  | string |  |  |  |  |
| `name` | Pricing Group | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `tname` |  | string |  |  |  |  |

## pricingGroupCollection

Browser definition `pricingGroupCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | pricingGroup[] |  |  | [`pricingGroup`](#pricinggroup) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |
