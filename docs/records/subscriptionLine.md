# subscriptionLine

Browser tag `subscriptionLine` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/subscriptionLine`, instance `/subscriptionLine/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/subscriptionLine` | `operation--subscriptionLine-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/subscriptionLine` | `operation--subscriptionLine-get` | Get list of records. |  | 200 OK → `subscriptionLineCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/subscriptionLine` | `operation--subscriptionLine-patch` | Update records. | `subscriptionLineCollection` | 202 Accepted; default → `nsError` |
| POST | `/subscriptionLine` | `operation--subscriptionLine-post` | Insert record. | `subscriptionLine` | 200 OK → `subscriptionLine`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/subscriptionLine` | `operation--subscriptionLine-put` | Insert or update records. | `subscriptionLineCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/subscriptionLine/{id}` | `operation--subscriptionLine--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/subscriptionLine/{id}` | `operation--subscriptionLine--id--get` | Get record. |  | 200 OK → `subscriptionLine`; 202 Accepted; default → `nsError` |
| PATCH | `/subscriptionLine/{id}` | `operation--subscriptionLine--id--patch` | Update record. | `subscriptionLine` | 200 OK → `subscriptionLine`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/subscriptionLine/{id}` | `operation--subscriptionLine--id--put` | Insert or update record. | `subscriptionLine` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--subscriptionLine-delete` | DELETE `/subscriptionLine` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subscriptionLine-get` | GET `/subscriptionLine` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subscriptionLine-patch` | PATCH `/subscriptionLine` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subscriptionLine-post` | POST `/subscriptionLine` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--subscriptionLine-put` | PUT `/subscriptionLine` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subscriptionLine--id--delete` | DELETE `/subscriptionLine/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subscriptionLine--id--get` | GET `/subscriptionLine/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subscriptionLine--id--patch` | PATCH `/subscriptionLine/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--subscriptionLine--id--put` | PUT `/subscriptionLine/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [subscriptionLine schemas](../schemas/subscriptionLine.md).

| Definition | Role |
| --- | --- |
| [`subscriptionLine`](../schemas/subscriptionLine.md#subscriptionline) | record body |
| [`subscriptionLineCollection`](../schemas/subscriptionLine.md#subscriptionlinecollection) | collection page |
| [`subscriptionLineSelectOptions`](../schemas/subscriptionLine.md#subscriptionlineselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
