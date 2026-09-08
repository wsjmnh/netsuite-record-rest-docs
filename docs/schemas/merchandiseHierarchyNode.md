# Schemas: merchandiseHierarchyNode

Property tables for definitions owned by `merchandiseHierarchyNode`.

Record page: [merchandiseHierarchyNode](../records/merchandiseHierarchyNode.md).

## Index

- [merchandiseHierarchyNode](#merchandisehierarchynode) — 8 properties
- [merchandiseHierarchyNode-hierarchyversionsCollection](#merchandisehierarchynode-hierarchyversionscollection) — 6 properties
- [merchandiseHierarchyNode-hierarchyversionsElement](#merchandisehierarchynode-hierarchyversionselement) — 10 properties
- [merchandiseHierarchyNodeCollection](#merchandisehierarchynodecollection) — 6 properties

## merchandiseHierarchyNode

Browser definition `merchandiseHierarchyNode`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `description` | Description | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `hierarchyversions` |  | merchandiseHierarchyNode-hierarchyversionsCollection |  |  | [`merchandiseHierarchyNode-hierarchyversionsCollection`](#merchandisehierarchynode-hierarchyversionscollection) |  |
| `id` | Internal ID | string |  |  |  |  |
| `internalId` | Internal ID | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## merchandiseHierarchyNode-hierarchyversionsCollection

Browser definition `merchandiseHierarchyNode-hierarchyversionsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | merchandiseHierarchyNode-hierarchyversionsElement[] |  |  | [`merchandiseHierarchyNode-hierarchyversionsElement`](#merchandisehierarchynode-hierarchyversionselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## merchandiseHierarchyNode-hierarchyversionsElement

Browser definition `merchandiseHierarchyNode-hierarchyversionsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `enddate` | Hierarchy Version End Date | string | date |  |  |  |
| `hierarchylevel` |  | merchandiseHierarchyLevel |  |  | [`merchandiseHierarchyLevel`](merchandiseHierarchyLevel.md#merchandisehierarchylevel) |  |
| `hierarchyversion` |  | merchandiseHierarchyVersion |  |  | [`merchandiseHierarchyVersion`](merchandiseHierarchyVersion.md#merchandisehierarchyversion) |  |
| `hierarchyversionid` | Hierarchy Version Id | integer | int64 |  |  |  |
| `isincluded` | Included In Version | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `parentnode` | Parent Node | string |  |  |  |  |
| `path` | Path | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `startdate` | Hierarchy Version Start Date | string | date |  |  |  |

## merchandiseHierarchyNodeCollection

Browser definition `merchandiseHierarchyNodeCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | merchandiseHierarchyNode[] |  |  | [`merchandiseHierarchyNode`](#merchandisehierarchynode) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |
