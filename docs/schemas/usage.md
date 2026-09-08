# Schemas: usage

Property tables for definitions owned by `usage`.

Record page: [usage](../records/usage.md).

## Index

- [usage](#usage) — 16 properties
- [usageCollection](#usagecollection) — 6 properties
- [usageSelectOptions](#usageselectoptions) — 7 properties

## usage

Browser definition `usage`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `customer` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `memo` | Memo | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `status` |  | object |  |  |  |  |
| `status.id` | Internal identifier | string |  |  |  | `ACTIVE`, `VOIDED` |
| `status.refName` | Reference Name | string |  |  |  |  |
| `subscriptionPlan` |  | subscriptionPlan |  |  | [`subscriptionPlan`](subscriptionPlan.md#subscriptionplan) |  |
| `usageDate` | Date | string | date |  |  |  |
| `usageQuantity` | Quantity | number | float |  |  |  |
| `usageSubscription` |  | subscription |  |  | [`subscription`](subscription.md#subscription) |  |
| `usageSubscriptionLine` |  | subscriptionLine |  |  | [`subscriptionLine`](subscriptionLine.md#subscriptionline) |  |

## usageCollection

Browser definition `usageCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | usage[] |  |  | [`usage`](#usage) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## usageSelectOptions

Browser definition `usageSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customer` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `item` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `status` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subscriptionPlan` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `usageSubscription` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `usageSubscriptionLine` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
