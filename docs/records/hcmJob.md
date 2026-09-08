# hcmJob

Browser tag `hcmJob` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/hcmJob`, instance `/hcmJob/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/hcmJob` | `operation--hcmJob-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/hcmJob` | `operation--hcmJob-get` | Get list of records. |  | 200 OK → `hcmJobCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/hcmJob` | `operation--hcmJob-patch` | Update records. | `hcmJobCollection` | 202 Accepted; default → `nsError` |
| POST | `/hcmJob` | `operation--hcmJob-post` | Insert record. | `hcmJob` | 200 OK → `hcmJob`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/hcmJob` | `operation--hcmJob-put` | Insert or update records. | `hcmJobCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/hcmJob/{id}` | `operation--hcmJob--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/hcmJob/{id}` | `operation--hcmJob--id--get` | Get record. |  | 200 OK → `hcmJob`; 202 Accepted; default → `nsError` |
| PATCH | `/hcmJob/{id}` | `operation--hcmJob--id--patch` | Update record. | `hcmJob` | 200 OK → `hcmJob`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/hcmJob/{id}` | `operation--hcmJob--id--put` | Insert or update record. | `hcmJob` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--hcmJob-delete` | DELETE `/hcmJob` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--hcmJob-get` | GET `/hcmJob` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--hcmJob-patch` | PATCH `/hcmJob` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--hcmJob-post` | POST `/hcmJob` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--hcmJob-put` | PUT `/hcmJob` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--hcmJob--id--delete` | DELETE `/hcmJob/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--hcmJob--id--get` | GET `/hcmJob/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--hcmJob--id--patch` | PATCH `/hcmJob/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--hcmJob--id--put` | PUT `/hcmJob/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [hcmJob schemas](../schemas/hcmJob.md).

| Definition | Role |
| --- | --- |
| [`hcmJob`](../schemas/hcmJob.md#hcmjob) | record body |
| [`hcmJobCollection`](../schemas/hcmJob.md#hcmjobcollection) | collection page |
| [`hcmJobSelectOptions`](../schemas/hcmJob.md#hcmjobselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
