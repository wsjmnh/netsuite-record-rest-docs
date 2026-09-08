# Schemas: merchandiseHierarchyVersion

Property tables for definitions owned by `merchandiseHierarchyVersion`.

Record page: [merchandiseHierarchyVersion](../records/merchandiseHierarchyVersion.md).

## Index

- [merchandiseHierarchyVersion](#merchandisehierarchyversion) — 10 properties
- [merchandiseHierarchyVersion-hierarchylevelsCollection](#merchandisehierarchyversion-hierarchylevelscollection) — 6 properties
- [merchandiseHierarchyVersion-hierarchylevelsElement](#merchandisehierarchyversion-hierarchylevelselement) — 5 properties
- [merchandiseHierarchyVersionCollection](#merchandisehierarchyversioncollection) — 6 properties

## merchandiseHierarchyVersion

Browser definition `merchandiseHierarchyVersion`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `description` | Description | string |  |  |  |  |
| `enddate` | End Date | string | date |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `hierarchylevels` |  | merchandiseHierarchyVersion-hierarchylevelsCollection |  |  | [`merchandiseHierarchyVersion-hierarchylevelsCollection`](#merchandisehierarchyversion-hierarchylevelscollection) |  |
| `id` | Internal ID | string |  |  |  |  |
| `internalId` | Internal ID | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `startdate` | Start Date | string | date |  |  |  |

## merchandiseHierarchyVersion-hierarchylevelsCollection

Browser definition `merchandiseHierarchyVersion-hierarchylevelsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | merchandiseHierarchyVersion-hierarchylevelsElement[] |  |  | [`merchandiseHierarchyVersion-hierarchylevelsElement`](#merchandisehierarchyversion-hierarchylevelselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## merchandiseHierarchyVersion-hierarchylevelsElement

Browser definition `merchandiseHierarchyVersion-hierarchylevelsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `hierarchylevel` |  | merchandiseHierarchyLevel |  |  | [`merchandiseHierarchyLevel`](merchandiseHierarchyLevel.md#merchandisehierarchylevel) |  |
| `isincluded` | Included In This Version | boolean |  |  |  |  |
| `levelrank` | Level Rank | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## merchandiseHierarchyVersionCollection

Browser definition `merchandiseHierarchyVersionCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | merchandiseHierarchyVersion[] |  |  | [`merchandiseHierarchyVersion`](#merchandisehierarchyversion) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |
