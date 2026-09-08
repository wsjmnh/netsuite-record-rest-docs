# Schemas: customerMessage

Property tables for definitions owned by `customerMessage`.

Record page: [customerMessage](../records/customerMessage.md).

## Index

- [customerMessage](#customermessage) — 8 properties
- [customerMessageCollection](#customermessagecollection) — 6 properties

## customerMessage

Browser definition `customerMessage`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `description` | Long Text | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Customer Message | string |  |  |  |  |
| `preferred` | Preferred | boolean |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## customerMessageCollection

Browser definition `customerMessageCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | customerMessage[] |  |  | [`customerMessage`](#customermessage) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |
