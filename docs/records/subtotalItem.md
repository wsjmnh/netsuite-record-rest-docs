# subtotalItem

Browser tag `subtotalItem` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/subtotalItem`, instance `/subtotalItem/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/subtotalItem` | `operation--subtotalItem-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/subtotalItem` | `operation--subtotalItem-get` | Get list of records. |  | 200 OK → `subtotalItemCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/subtotalItem` | `operation--subtotalItem-patch` | Update records. | `subtotalItemCollection` | 202 Accepted; default → `nsError` |
| POST | `/subtotalItem` | `operation--subtotalItem-post` | Insert record. | `subtotalItem` | 200 OK → `subtotalItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/subtotalItem` | `operation--subtotalItem-put` | Insert or update records. | `subtotalItemCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/subtotalItem/{id}` | `operation--subtotalItem--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/subtotalItem/{id}` | `operation--subtotalItem--id--get` | Get record. |  | 200 OK → `subtotalItem`; 202 Accepted; default → `nsError` |
| PATCH | `/subtotalItem/{id}` | `operation--subtotalItem--id--patch` | Update record. | `subtotalItem` | 200 OK → `subtotalItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/subtotalItem/{id}` | `operation--subtotalItem--id--put` | Insert or update record. | `subtotalItem` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--subtotalItem-delete` | DELETE `/subtotalItem` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subtotalItem-get` | GET `/subtotalItem` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subtotalItem-patch` | PATCH `/subtotalItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subtotalItem-post` | POST `/subtotalItem` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--subtotalItem-put` | PUT `/subtotalItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subtotalItem--id--delete` | DELETE `/subtotalItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subtotalItem--id--get` | GET `/subtotalItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subtotalItem--id--patch` | PATCH `/subtotalItem/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--subtotalItem--id--put` | PUT `/subtotalItem/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [subtotalItem schemas](../schemas/subtotalItem.md).

| Definition | Role |
| --- | --- |
| [`subtotalItem`](../schemas/subtotalItem.md#subtotalitem) | record body |
| [`subtotalItem-translationsCollection`](../schemas/subtotalItem.md#subtotalitem-translationscollection) | sublist/collection |
| [`subtotalItem-translationsElement`](../schemas/subtotalItem.md#subtotalitem-translationselement) | sublist/element |
| [`subtotalItemCollection`](../schemas/subtotalItem.md#subtotalitemcollection) | collection page |
| [`subtotalItemSelectOptions`](../schemas/subtotalItem.md#subtotalitemselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `translations` | [`subtotalItem-translationsCollection`](../schemas/subtotalItem.md#subtotalitem-translationscollection) | [`subtotalItem-translationsElement`](../schemas/subtotalItem.md#subtotalitem-translationselement) |
