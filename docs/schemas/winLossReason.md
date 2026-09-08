# Schemas: winLossReason

Property tables for definitions owned by `winLossReason`.

Record page: [winLossReason](../records/winLossReason.md).

## Index

- [winLossReason](#winlossreason) — 6 properties
- [winLossReasonCollection](#winlossreasoncollection) — 6 properties

## winLossReason

Browser definition `winLossReason`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Reason | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## winLossReasonCollection

Browser definition `winLossReasonCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | winLossReason[] |  |  | [`winLossReason`](#winlossreason) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |
