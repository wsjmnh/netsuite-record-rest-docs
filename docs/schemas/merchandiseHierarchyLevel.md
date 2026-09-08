# Schemas: merchandiseHierarchyLevel

Property tables for definitions owned by `merchandiseHierarchyLevel`.

Record page: [merchandiseHierarchyLevel](../records/merchandiseHierarchyLevel.md).

## Index

- [merchandiseHierarchyLevel](#merchandisehierarchylevel) — 9 properties
- [merchandiseHierarchyLevelCollection](#merchandisehierarchylevelcollection) — 6 properties
- [merchandiseHierarchyLevelSelectOptions](#merchandisehierarchylevelselectoptions) — 1 properties

## merchandiseHierarchyLevel

Browser definition `merchandiseHierarchyLevel`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `description` | Description | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `insertbefore` |  | merchandiseHierarchyLevel |  |  | [`merchandiseHierarchyLevel`](#merchandisehierarchylevel) |  |
| `internalId` | Internal ID | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Name | string |  |  |  |  |
| `rank` | Rank | integer | int64 |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## merchandiseHierarchyLevelCollection

Browser definition `merchandiseHierarchyLevelCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | merchandiseHierarchyLevel[] |  |  | [`merchandiseHierarchyLevel`](#merchandisehierarchylevel) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## merchandiseHierarchyLevelSelectOptions

Browser definition `merchandiseHierarchyLevelSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `insertbefore` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
