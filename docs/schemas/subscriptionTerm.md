# Schemas: subscriptionTerm

Property tables for definitions owned by `subscriptionTerm`.

Record page: [subscriptionTerm](../records/subscriptionTerm.md).

## Index

- [subscriptionTerm](#subscriptionterm) — 15 properties
- [subscriptionTermCollection](#subscriptiontermcollection) — 6 properties
- [subscriptionTermSelectOptions](#subscriptiontermselectoptions) — 2 properties

## subscriptionTerm

Browser definition `subscriptionTerm`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `longitemtype` |  | string |  |  |  |  |
| `name` | Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `subscriptionTermDuration` | Duration | integer | int64 |  |  |  |
| `subscriptionTermType` |  | object |  |  |  |  |
| `subscriptionTermType.id` | Internal identifier | string |  |  |  | `EVERGREEN`, `CUSTOM`, `STANDARD` |
| `subscriptionTermType.refName` | Reference Name | string |  |  |  |  |
| `subscriptionTermUnit` |  | object |  |  |  |  |
| `subscriptionTermUnit.id` | Internal identifier | string |  |  |  | `YEARS`, `MONTHS`, `WEEKS`, `DAYS` |
| `subscriptionTermUnit.refName` | Reference Name | string |  |  |  |  |
| `tname` |  | string |  |  |  |  |

## subscriptionTermCollection

Browser definition `subscriptionTermCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | subscriptionTerm[] |  |  | [`subscriptionTerm`](#subscriptionterm) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## subscriptionTermSelectOptions

Browser definition `subscriptionTermSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `subscriptionTermType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subscriptionTermUnit` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
