# Schemas: vendorCategory

Property tables for definitions owned by `vendorCategory`.

Record page: [vendorCategory](../records/vendorCategory.md).

## Index

- [vendorCategory](#vendorcategory) — 10 properties
- [vendorCategoryCollection](#vendorcategorycollection) — 6 properties

## vendorCategory

Browser definition `vendorCategory`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `isTaxAgency` | Tax Agency | boolean |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `longitemtype` |  | string |  |  |  |  |
| `name` | Vendor | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `tname` |  | string |  |  |  |  |

## vendorCategoryCollection

Browser definition `vendorCategoryCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | vendorCategory[] |  |  | [`vendorCategory`](#vendorcategory) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |
