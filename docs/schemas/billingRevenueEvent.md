# Schemas: billingRevenueEvent

Property tables for definitions owned by `billingRevenueEvent`.

Record page: [billingRevenueEvent](../records/billingRevenueEvent.md).

## Index

- [billingRevenueEvent](#billingrevenueevent) — 20 properties
- [billingRevenueEventCollection](#billingrevenueeventcollection) — 6 properties
- [billingRevenueEventSelectOptions](#billingrevenueeventselectoptions) — 6 properties

## billingRevenueEvent

Browser definition `billingRevenueEvent`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amount` | Amount (Transaction Currency) | number | double |  |  |  |
| `cumulativePercentComplete` | Cumulative Percent Complete | number | double |  |  |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `endDate` | End Date | string | date |  |  |  |
| `eventDate` | Date | string | date |  |  |  |
| `eventPurpose` |  | object |  |  |  |  |
| `eventPurpose.id` | Internal identifier | string |  |  |  | `FORECAST`, `ACTUAL` |
| `eventPurpose.refName` | Reference Name | string |  |  |  |  |
| `eventType` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `projectRevenueRule` |  | object |  |  |  |  |
| `projectRevenueRule.id` | Internal identifier | string |  |  |  |  |
| `projectRevenueRule.refName` | Reference Name | string |  |  |  |  |
| `quantity` | Quantity | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `startDate` | Start Date | string | date |  |  |  |
| `subscriptionLine` |  | subscriptionLine |  |  | [`subscriptionLine`](subscriptionLine.md#subscriptionline) |  |
| `transactionLine` | Transaction Line | string |  |  |  |  |

## billingRevenueEventCollection

Browser definition `billingRevenueEventCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | billingRevenueEvent[] |  |  | [`billingRevenueEvent`](#billingrevenueevent) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## billingRevenueEventSelectOptions

Browser definition `billingRevenueEventSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `eventPurpose` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `eventType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `projectRevenueRule` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subscriptionLine` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `transactionLine` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
