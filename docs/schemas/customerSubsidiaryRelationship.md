# Schemas: customerSubsidiaryRelationship

Property tables for definitions owned by `customerSubsidiaryRelationship`.

Record page: [customerSubsidiaryRelationship](../records/customerSubsidiaryRelationship.md).

## Index

- [customerSubsidiaryRelationship](#customersubsidiaryrelationship) — 13 properties
- [customerSubsidiaryRelationshipCollection](#customersubsidiaryrelationshipcollection) — 6 properties
- [customerSubsidiaryRelationshipSelectOptions](#customersubsidiaryrelationshipselectoptions) — 3 properties

## customerSubsidiaryRelationship

Browser definition `customerSubsidiaryRelationship`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `balance` | Balance | number | double |  |  |  |
| `depositBalance` | Deposit Balance | number | double |  |  |  |
| `entity` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isPrimarySub` | Is Primary Subsidiary | boolean |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Name | string |  |  |  |  |
| `primaryCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `unbilledOrders` | Unbilled Orders | number | double |  |  |  |

## customerSubsidiaryRelationshipCollection

Browser definition `customerSubsidiaryRelationshipCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | customerSubsidiaryRelationship[] |  |  | [`customerSubsidiaryRelationship`](#customersubsidiaryrelationship) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## customerSubsidiaryRelationshipSelectOptions

Browser definition `customerSubsidiaryRelationshipSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `entity` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `primaryCurrency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
