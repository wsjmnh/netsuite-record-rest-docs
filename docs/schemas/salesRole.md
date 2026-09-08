# Schemas: salesRole

Property tables for definitions owned by `salesRole`.

Record page: [salesRole](../records/salesRole.md).

## Index

- [salesRole](#salesrole) — 8 properties
- [salesRoleCollection](#salesrolecollection) — 6 properties

## salesRole

Browser definition `salesRole`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `description` | Description | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `isSalesRep` | Sales Rep | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Role | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## salesRoleCollection

Browser definition `salesRoleCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | salesRole[] |  |  | [`salesRole`](#salesrole) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |
