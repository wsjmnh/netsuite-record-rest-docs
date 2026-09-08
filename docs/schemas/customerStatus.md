# Schemas: customerStatus

Property tables for definitions owned by `customerStatus`.

Record page: [customerStatus](../records/customerStatus.md).

## Index

- [customerStatus](#customerstatus) — 12 properties
- [customerStatusCollection](#customerstatuscollection) — 6 properties
- [customerStatusSelectOptions](#customerstatusselectoptions) — 1 properties

## customerStatus

Browser definition `customerStatus`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `description` | Description | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `includeInLeadReports` | Include In Lead Reports | boolean |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Status | string |  |  |  |  |
| `probability` | Probability | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `stage` |  | object |  |  |  |  |
| `stage.id` | Internal identifier | string |  |  |  | `CUSTOMER`, `PROSPECT`, `LEAD` |
| `stage.refName` | Reference Name | string |  |  |  |  |

## customerStatusCollection

Browser definition `customerStatusCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | customerStatus[] |  |  | [`customerStatus`](#customerstatus) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## customerStatusSelectOptions

Browser definition `customerStatusSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `stage` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
