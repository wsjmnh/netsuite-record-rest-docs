# Schemas: vendorSubsidiaryRelationship

Property tables for definitions owned by `vendorSubsidiaryRelationship`.

Record page: [vendorSubsidiaryRelationship](../records/vendorSubsidiaryRelationship.md).

## Index

- [vendorSubsidiaryRelationship](#vendorsubsidiaryrelationship) — 21 properties
- [vendorSubsidiaryRelationshipCollection](#vendorsubsidiaryrelationshipcollection) — 6 properties
- [vendorSubsidiaryRelationshipSelectOptions](#vendorsubsidiaryrelationshipselectoptions) — 5 properties

## vendorSubsidiaryRelationship

Browser definition `vendorSubsidiaryRelationship`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `balance` | Balance | number | double |  |  |  |
| `balanceBase` | Balance (Base) | number | double |  |  |  |
| `baseCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `baseInTransitBalance` | In-Transit Balance (Base) | number | double |  |  |  |
| `creditLimit` | Credit Limit | number | double |  |  |  |
| `entity` |  | vendor |  |  | [`vendor`](vendor.md#vendor) |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `inTransitBalance` | In-Transit Balance | number | double |  |  |  |
| `isPrimarySub` | Is Primary Subsidiary | boolean |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Name | string |  |  |  |  |
| `prepaymentBalance` | Prepayment Balance | number | double |  |  |  |
| `prepaymentBalanceBase` | Prepayment Balance (Base) | number | double |  |  |  |
| `primaryCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `taxItem` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `unbilledOrders` | Unbilled Orders | number | double |  |  |  |
| `unbilledOrdersBase` | Unbilled Orders (Base) | number | double |  |  |  |

## vendorSubsidiaryRelationshipCollection

Browser definition `vendorSubsidiaryRelationshipCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | vendorSubsidiaryRelationship[] |  |  | [`vendorSubsidiaryRelationship`](#vendorsubsidiaryrelationship) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## vendorSubsidiaryRelationshipSelectOptions

Browser definition `vendorSubsidiaryRelationshipSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `baseCurrency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `entity` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `primaryCurrency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `taxItem` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
