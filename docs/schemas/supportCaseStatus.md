# Schemas: supportCaseStatus

Property tables for definitions owned by `supportCaseStatus`.

Record page: [supportCaseStatus](../records/supportCaseStatus.md).

## Index

- [supportCaseStatus](#supportcasestatus) — 15 properties
- [supportCaseStatusCollection](#supportcasestatuscollection) — 6 properties
- [supportCaseStatusSelectOptions](#supportcasestatusselectoptions) — 2 properties

## supportCaseStatus

Browser definition `supportCaseStatus`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `autoCloseCase` | Auto Close With Issues | boolean |  |  |  |  |
| `caseOnHold` | On Hold | boolean |  |  |  |  |
| `description` | Description | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `insertBefore` |  | supportCaseStatus |  |  | [`supportCaseStatus`](#supportcasestatus) |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Case Status | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `showAwaitingReply` | Show Awaiting Support Reply | boolean |  |  |  |  |
| `sortOrder` | Sort Order | integer | int64 |  |  |  |
| `stage` |  | object |  |  |  |  |
| `stage.id` | Internal identifier | string |  |  |  | `OPEN`, `ESCALATED`, `CLOSED` |
| `stage.refName` | Reference Name | string |  |  |  |  |

## supportCaseStatusCollection

Browser definition `supportCaseStatusCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | supportCaseStatus[] |  |  | [`supportCaseStatus`](#supportcasestatus) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## supportCaseStatusSelectOptions

Browser definition `supportCaseStatusSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `insertBefore` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `stage` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
