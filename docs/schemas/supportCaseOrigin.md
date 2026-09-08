# Schemas: supportCaseOrigin

Property tables for definitions owned by `supportCaseOrigin`.

Record page: [supportCaseOrigin](../records/supportCaseOrigin.md).

## Index

- [supportCaseOrigin](#supportcaseorigin) — 10 properties
- [supportCaseOriginCollection](#supportcaseorigincollection) — 6 properties
- [supportCaseOriginSelectOptions](#supportcaseoriginselectoptions) — 1 properties

## supportCaseOrigin

Browser definition `supportCaseOrigin`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `description` | Description | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `insertBefore` |  | supportCaseOrigin |  |  | [`supportCaseOrigin`](#supportcaseorigin) |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Case Origin | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `sortOrder` | Sort Order | integer | int64 |  |  |  |

## supportCaseOriginCollection

Browser definition `supportCaseOriginCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | supportCaseOrigin[] |  |  | [`supportCaseOrigin`](#supportcaseorigin) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## supportCaseOriginSelectOptions

Browser definition `supportCaseOriginSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `insertBefore` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
