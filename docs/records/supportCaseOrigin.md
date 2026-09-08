# supportCaseOrigin

Browser tag `supportCaseOrigin` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/supportCaseOrigin`, instance `/supportCaseOrigin/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/supportCaseOrigin` | `operation--supportCaseOrigin-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/supportCaseOrigin` | `operation--supportCaseOrigin-get` | Get list of records. |  | 200 OK → `supportCaseOriginCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/supportCaseOrigin` | `operation--supportCaseOrigin-patch` | Update records. | `supportCaseOriginCollection` | 202 Accepted; default → `nsError` |
| POST | `/supportCaseOrigin` | `operation--supportCaseOrigin-post` | Insert record. | `supportCaseOrigin` | 200 OK → `supportCaseOrigin`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/supportCaseOrigin` | `operation--supportCaseOrigin-put` | Insert or update records. | `supportCaseOriginCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/supportCaseOrigin/{id}` | `operation--supportCaseOrigin--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/supportCaseOrigin/{id}` | `operation--supportCaseOrigin--id--get` | Get record. |  | 200 OK → `supportCaseOrigin`; 202 Accepted; default → `nsError` |
| PATCH | `/supportCaseOrigin/{id}` | `operation--supportCaseOrigin--id--patch` | Update record. | `supportCaseOrigin` | 200 OK → `supportCaseOrigin`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/supportCaseOrigin/{id}` | `operation--supportCaseOrigin--id--put` | Insert or update record. | `supportCaseOrigin` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--supportCaseOrigin-delete` | DELETE `/supportCaseOrigin` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--supportCaseOrigin-get` | GET `/supportCaseOrigin` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--supportCaseOrigin-patch` | PATCH `/supportCaseOrigin` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--supportCaseOrigin-post` | POST `/supportCaseOrigin` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--supportCaseOrigin-put` | PUT `/supportCaseOrigin` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--supportCaseOrigin--id--delete` | DELETE `/supportCaseOrigin/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--supportCaseOrigin--id--get` | GET `/supportCaseOrigin/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--supportCaseOrigin--id--patch` | PATCH `/supportCaseOrigin/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--supportCaseOrigin--id--put` | PUT `/supportCaseOrigin/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [supportCaseOrigin schemas](../schemas/supportCaseOrigin.md).

| Definition | Role |
| --- | --- |
| [`supportCaseOrigin`](../schemas/supportCaseOrigin.md#supportcaseorigin) | record body |
| [`supportCaseOriginCollection`](../schemas/supportCaseOrigin.md#supportcaseorigincollection) | collection page |
| [`supportCaseOriginSelectOptions`](../schemas/supportCaseOrigin.md#supportcaseoriginselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
