# Schemas: contactCategory

Property tables for definitions owned by `contactCategory`.

Record page: [contactCategory](../records/contactCategory.md).

## Index

- [contactCategory](#contactcategory) — 7 properties
- [contactCategoryCollection](#contactcategorycollection) — 6 properties

## contactCategory

Browser definition `contactCategory`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Contact Category | string |  |  |  |  |
| `private` | Private | boolean |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## contactCategoryCollection

Browser definition `contactCategoryCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | contactCategory[] |  |  | [`contactCategory`](#contactcategory) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |
