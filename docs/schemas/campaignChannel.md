# Schemas: campaignChannel

Property tables for definitions owned by `campaignChannel`.

Record page: [campaignChannel](../records/campaignChannel.md).

## Index

- [campaignChannel](#campaignchannel) — 10 properties
- [campaignChannelCollection](#campaignchannelcollection) — 6 properties
- [campaignChannelSelectOptions](#campaignchannelselectoptions) — 1 properties

## campaignChannel

Browser definition `campaignChannel`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `description` | Description | string |  |  |  |  |
| `eventType` |  | object |  |  |  |  |
| `eventType.id` | Internal identifier | string |  |  |  | `OTHER`, `INTEGRATION`, `DRIP`, `EMAIL`, `DIRECTMAIL` |
| `eventType.refName` | Reference Name | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## campaignChannelCollection

Browser definition `campaignChannelCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | campaignChannel[] |  |  | [`campaignChannel`](#campaignchannel) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## campaignChannelSelectOptions

Browser definition `campaignChannelSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `eventType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
