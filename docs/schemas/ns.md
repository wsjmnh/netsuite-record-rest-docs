# Schemas: ns

Shared `ns*` definitions used across record resources.

## Index

- [nsError](#nserror) — 10 properties
- [nsLink](#nslink) — 2 properties
- [nsResource](#nsresource) — 4 properties
- [nsResourceCollection](#nsresourcecollection) — 6 properties
- [nsResourceSelectOptions](#nsresourceselectoptions) — 1 properties

## nsError

Browser definition `nsError`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `o:errorDetails` |  | object[] |  | read-only |  |  |
| `o:errorDetails[].detail` | Detail | string |  | read-only |  |  |
| `o:errorDetails[].o:errorCode` | Error Code | string |  | read-only |  |  |
| `o:errorDetails[].o:errorHeader` | Error Header | string |  | read-only |  |  |
| `o:errorDetails[].o:errorPath` | Error Path | string | JSONPath | read-only |  |  |
| `o:errorDetails[].o:errorQueryParam` | Error Query Parameter | string |  | read-only |  |  |
| `o:errorDetails[].o:errorUrl` | Error URL | string | URI | read-only |  |  |
| `status` | Status | integer | int32 | read-only |  |  |
| `title` | Title | string |  | read-only |  |  |
| `type` | Type | string | URI | read-only |  |  |

## nsLink

Browser definition `nsLink`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `href` | Hypertext Reference | string |  | read-only |  |  |
| `rel` | Relationship | string |  | read-only |  |  |

## nsResource

Browser definition `nsResource`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `externalId` | External identifier | string |  |  |  |  |
| `id` | Internal identifier | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## nsResourceCollection

Browser definition `nsResourceCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | nsResource[] |  |  | [`nsResource`](#nsresource) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## nsResourceSelectOptions

Browser definition `nsResourceSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `_selectOptions` |  | nsResource[] |  |  | [`nsResource`](#nsresource) |  |
