# Schemas: campaignSubscription

Property tables for definitions owned by `campaignSubscription`.

Record page: [campaignSubscription](../records/campaignSubscription.md).

## Index

- [campaignSubscription](#campaignsubscription) — 10 properties
- [campaignSubscriptionCollection](#campaignsubscriptioncollection) — 6 properties

## campaignSubscription

Browser definition `campaignSubscription`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `description` | Description | string |  |  |  |  |
| `externalDescription` | External Description | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `externalName` | External Name | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `subscribedByDefault` | Subscribed by Default | boolean |  |  |  |  |

## campaignSubscriptionCollection

Browser definition `campaignSubscriptionCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | campaignSubscription[] |  |  | [`campaignSubscription`](#campaignsubscription) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |
