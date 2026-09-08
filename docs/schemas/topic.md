# Schemas: topic

Property tables for definitions owned by `topic`.

Record page: [topic](../records/topic.md).

## Index

- [topic](#topic) — 9 properties
- [topicCollection](#topiccollection) — 6 properties
- [topicSelectOptions](#topicselectoptions) — 1 properties

## topic

Browser definition `topic`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `description` | Brief Description | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `longDescription` | Detailed Description | string |  |  |  |  |
| `parentTopic` |  | topic |  |  | [`topic`](#topic) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `title` | Title | string |  |  |  |  |

## topicCollection

Browser definition `topicCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | topic[] |  |  | [`topic`](#topic) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## topicSelectOptions

Browser definition `topicSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `parentTopic` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
