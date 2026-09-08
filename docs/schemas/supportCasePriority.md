# Schemas: supportCasePriority

Property tables for definitions owned by `supportCasePriority`.

Record page: [supportCasePriority](../records/supportCasePriority.md).

## Index

- [supportCasePriority](#supportcasepriority) — 9 properties
- [supportCasePriorityCollection](#supportcaseprioritycollection) — 6 properties
- [supportCasePrioritySelectOptions](#supportcasepriorityselectoptions) — 1 properties

## supportCasePriority

Browser definition `supportCasePriority`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `description` | Description | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `insertBefore` |  | supportCasePriority |  |  | [`supportCasePriority`](#supportcasepriority) |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Case Priority | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `sortOrder` | Sort Order | integer | int64 |  |  |  |

## supportCasePriorityCollection

Browser definition `supportCasePriorityCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | supportCasePriority[] |  |  | [`supportCasePriority`](#supportcasepriority) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## supportCasePrioritySelectOptions

Browser definition `supportCasePrioritySelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `insertBefore` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
