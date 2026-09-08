# Schemas: jobType

Property tables for definitions owned by `jobType`.

Record page: [jobType](../records/jobType.md).

## Index

- [jobType](#jobtype) — 7 properties
- [jobTypeCollection](#jobtypecollection) — 6 properties
- [jobTypeSelectOptions](#jobtypeselectoptions) — 1 properties

## jobType

Browser definition `jobType`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Project Type | string |  |  |  |  |
| `parent` |  | jobType |  |  | [`jobType`](#jobtype) |  |
| `refName` | Reference Name | string |  |  |  |  |

## jobTypeCollection

Browser definition `jobTypeCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | jobType[] |  |  | [`jobType`](#jobtype) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## jobTypeSelectOptions

Browser definition `jobTypeSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `parent` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
