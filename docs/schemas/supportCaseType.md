# Schemas: supportCaseType

Property tables for definitions owned by `supportCaseType`.

Record page: [supportCaseType](../records/supportCaseType.md).

## Index

- [supportCaseType](#supportcasetype) — 10 properties
- [supportCaseTypeCollection](#supportcasetypecollection) — 6 properties
- [supportCaseTypeSelectOptions](#supportcasetypeselectoptions) — 1 properties

## supportCaseType

Browser definition `supportCaseType`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `description` | Description | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `insertBefore` |  | supportCaseType |  |  | [`supportCaseType`](#supportcasetype) |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Case Type | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `sortOrder` | Sort Order | integer | int64 |  |  |  |

## supportCaseTypeCollection

Browser definition `supportCaseTypeCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | supportCaseType[] |  |  | [`supportCaseType`](#supportcasetype) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## supportCaseTypeSelectOptions

Browser definition `supportCaseTypeSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `insertBefore` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
