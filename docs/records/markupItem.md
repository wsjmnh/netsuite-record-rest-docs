# markupItem

Browser tag `markupItem` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/markupItem`, instance `/markupItem/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/markupItem` | `operation--markupItem-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/markupItem` | `operation--markupItem-get` | Get list of records. |  | 200 OK → `markupItemCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/markupItem` | `operation--markupItem-patch` | Update records. | `markupItemCollection` | 202 Accepted; default → `nsError` |
| POST | `/markupItem` | `operation--markupItem-post` | Insert record. | `markupItem` | 200 OK → `markupItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/markupItem` | `operation--markupItem-put` | Insert or update records. | `markupItemCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/markupItem/{id}` | `operation--markupItem--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/markupItem/{id}` | `operation--markupItem--id--get` | Get record. |  | 200 OK → `markupItem`; 202 Accepted; default → `nsError` |
| PATCH | `/markupItem/{id}` | `operation--markupItem--id--patch` | Update record. | `markupItem` | 200 OK → `markupItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/markupItem/{id}` | `operation--markupItem--id--put` | Insert or update record. | `markupItem` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--markupItem-delete` | DELETE `/markupItem` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--markupItem-get` | GET `/markupItem` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--markupItem-patch` | PATCH `/markupItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--markupItem-post` | POST `/markupItem` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--markupItem-put` | PUT `/markupItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--markupItem--id--delete` | DELETE `/markupItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--markupItem--id--get` | GET `/markupItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--markupItem--id--patch` | PATCH `/markupItem/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--markupItem--id--put` | PUT `/markupItem/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [markupItem schemas](../schemas/markupItem.md).

| Definition | Role |
| --- | --- |
| [`markupItem`](../schemas/markupItem.md#markupitem) | record body |
| [`markupItem-translationsCollection`](../schemas/markupItem.md#markupitem-translationscollection) | sublist/collection |
| [`markupItem-translationsElement`](../schemas/markupItem.md#markupitem-translationselement) | sublist/element |
| [`markupItemCollection`](../schemas/markupItem.md#markupitemcollection) | collection page |
| [`markupItemSelectOptions`](../schemas/markupItem.md#markupitemselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `translations` | [`markupItem-translationsCollection`](../schemas/markupItem.md#markupitem-translationscollection) | [`markupItem-translationsElement`](../schemas/markupItem.md#markupitem-translationselement) |
