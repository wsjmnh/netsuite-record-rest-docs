# Schemas: hcmJob

Property tables for definitions owned by `hcmJob`.

Record page: [hcmJob](../records/hcmJob.md).

## Index

- [hcmJob](#hcmjob) — 13 properties
- [hcmJobCollection](#hcmjobcollection) — 6 properties
- [hcmJobSelectOptions](#hcmjobselectoptions) — 1 properties

## hcmJob

Browser definition `hcmJob`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `description` | Description | string |  |  |  |  |
| `employmentCategory` |  | object |  |  |  |  |
| `employmentCategory.id` | Internal identifier | string |  |  |  | `-10`, `-11` |
| `employmentCategory.refName` | Reference Name | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `internalId` | Internal ID | integer | int64 |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `jobid` | Job ID | string |  |  |  |  |
| `jobidlabel` | Job ID | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `title` | Title | string |  |  |  |  |

## hcmJobCollection

Browser definition `hcmJobCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | hcmJob[] |  |  | [`hcmJob`](#hcmjob) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## hcmJobSelectOptions

Browser definition `hcmJobSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `employmentCategory` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
