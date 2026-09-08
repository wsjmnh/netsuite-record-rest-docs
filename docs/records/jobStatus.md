# jobStatus

Browser tag `jobStatus` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/jobStatus`, instance `/jobStatus/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/jobStatus` | `operation--jobStatus-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/jobStatus` | `operation--jobStatus-get` | Get list of records. |  | 200 OK → `jobStatusCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/jobStatus` | `operation--jobStatus-patch` | Update records. | `jobStatusCollection` | 202 Accepted; default → `nsError` |
| POST | `/jobStatus` | `operation--jobStatus-post` | Insert record. | `jobStatus` | 200 OK → `jobStatus`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/jobStatus` | `operation--jobStatus-put` | Insert or update records. | `jobStatusCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/jobStatus/{id}` | `operation--jobStatus--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/jobStatus/{id}` | `operation--jobStatus--id--get` | Get record. |  | 200 OK → `jobStatus`; 202 Accepted; default → `nsError` |
| PATCH | `/jobStatus/{id}` | `operation--jobStatus--id--patch` | Update record. | `jobStatus` | 200 OK → `jobStatus`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/jobStatus/{id}` | `operation--jobStatus--id--put` | Insert or update record. | `jobStatus` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--jobStatus-delete` | DELETE `/jobStatus` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--jobStatus-get` | GET `/jobStatus` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--jobStatus-patch` | PATCH `/jobStatus` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--jobStatus-post` | POST `/jobStatus` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--jobStatus-put` | PUT `/jobStatus` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--jobStatus--id--delete` | DELETE `/jobStatus/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--jobStatus--id--get` | GET `/jobStatus/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--jobStatus--id--patch` | PATCH `/jobStatus/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--jobStatus--id--put` | PUT `/jobStatus/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [jobStatus schemas](../schemas/jobStatus.md).

| Definition | Role |
| --- | --- |
| [`jobStatus`](../schemas/jobStatus.md#jobstatus) | record body |
| [`jobStatusCollection`](../schemas/jobStatus.md#jobstatuscollection) | collection page |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
