# Schemas: campaignCategory

Property tables for definitions owned by `campaignCategory`.

Record page: [campaignCategory](../records/campaignCategory.md).

## Index

- [campaignCategory](#campaigncategory) — 12 properties
- [campaignCategoryCollection](#campaigncategorycollection) — 6 properties
- [campaignCategorySelectOptions](#campaigncategoryselectoptions) — 2 properties

## campaignCategory

Browser definition `campaignCategory`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `description` | Description | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `fullName` | Full Name | string |  |  |  |  |
| `hierarchyRawFullName` | Full Name (Raw) | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isExternal` | Available Externally | boolean |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `leadSource` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Name | string |  |  |  |  |
| `parent` |  | campaignCategory |  |  | [`campaignCategory`](#campaigncategory) |  |
| `refName` | Reference Name | string |  |  |  |  |

## campaignCategoryCollection

Browser definition `campaignCategoryCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | campaignCategory[] |  |  | [`campaignCategory`](#campaigncategory) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## campaignCategorySelectOptions

Browser definition `campaignCategorySelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `leadSource` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `parent` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
