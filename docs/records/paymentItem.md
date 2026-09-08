# paymentItem

Browser tag `paymentItem` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/paymentItem`, instance `/paymentItem/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/paymentItem` | `operation--paymentItem-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/paymentItem` | `operation--paymentItem-get` | Get list of records. |  | 200 OK → `paymentItemCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/paymentItem` | `operation--paymentItem-patch` | Update records. | `paymentItemCollection` | 202 Accepted; default → `nsError` |
| POST | `/paymentItem` | `operation--paymentItem-post` | Insert record. | `paymentItem` | 200 OK → `paymentItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/paymentItem` | `operation--paymentItem-put` | Insert or update records. | `paymentItemCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/paymentItem/{id}` | `operation--paymentItem--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/paymentItem/{id}` | `operation--paymentItem--id--get` | Get record. |  | 200 OK → `paymentItem`; 202 Accepted; default → `nsError` |
| PATCH | `/paymentItem/{id}` | `operation--paymentItem--id--patch` | Update record. | `paymentItem` | 200 OK → `paymentItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/paymentItem/{id}` | `operation--paymentItem--id--put` | Insert or update record. | `paymentItem` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--paymentItem-delete` | DELETE `/paymentItem` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--paymentItem-get` | GET `/paymentItem` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--paymentItem-patch` | PATCH `/paymentItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--paymentItem-post` | POST `/paymentItem` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--paymentItem-put` | PUT `/paymentItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--paymentItem--id--delete` | DELETE `/paymentItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--paymentItem--id--get` | GET `/paymentItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--paymentItem--id--patch` | PATCH `/paymentItem/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--paymentItem--id--put` | PUT `/paymentItem/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [paymentItem schemas](../schemas/paymentItem.md).

| Definition | Role |
| --- | --- |
| [`paymentItem`](../schemas/paymentItem.md#paymentitem) | record body |
| [`paymentItem-translationsCollection`](../schemas/paymentItem.md#paymentitem-translationscollection) | sublist/collection |
| [`paymentItem-translationsElement`](../schemas/paymentItem.md#paymentitem-translationselement) | sublist/element |
| [`paymentItemCollection`](../schemas/paymentItem.md#paymentitemcollection) | collection page |
| [`paymentItemSelectOptions`](../schemas/paymentItem.md#paymentitemselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `translations` | [`paymentItem-translationsCollection`](../schemas/paymentItem.md#paymentitem-translationscollection) | [`paymentItem-translationsElement`](../schemas/paymentItem.md#paymentitem-translationselement) |
