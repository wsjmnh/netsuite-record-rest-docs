# supportCaseStatus

Browser tag `supportCaseStatus` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/supportCaseStatus`, instance `/supportCaseStatus/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/supportCaseStatus` | `operation--supportCaseStatus-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/supportCaseStatus` | `operation--supportCaseStatus-get` | Get list of records. |  | 200 OK → `supportCaseStatusCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/supportCaseStatus` | `operation--supportCaseStatus-patch` | Update records. | `supportCaseStatusCollection` | 202 Accepted; default → `nsError` |
| POST | `/supportCaseStatus` | `operation--supportCaseStatus-post` | Insert record. | `supportCaseStatus` | 200 OK → `supportCaseStatus`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/supportCaseStatus` | `operation--supportCaseStatus-put` | Insert or update records. | `supportCaseStatusCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/supportCaseStatus/{id}` | `operation--supportCaseStatus--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/supportCaseStatus/{id}` | `operation--supportCaseStatus--id--get` | Get record. |  | 200 OK → `supportCaseStatus`; 202 Accepted; default → `nsError` |
| PATCH | `/supportCaseStatus/{id}` | `operation--supportCaseStatus--id--patch` | Update record. | `supportCaseStatus` | 200 OK → `supportCaseStatus`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/supportCaseStatus/{id}` | `operation--supportCaseStatus--id--put` | Insert or update record. | `supportCaseStatus` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--supportCaseStatus-delete` | DELETE `/supportCaseStatus` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--supportCaseStatus-get` | GET `/supportCaseStatus` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--supportCaseStatus-patch` | PATCH `/supportCaseStatus` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--supportCaseStatus-post` | POST `/supportCaseStatus` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--supportCaseStatus-put` | PUT `/supportCaseStatus` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--supportCaseStatus--id--delete` | DELETE `/supportCaseStatus/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--supportCaseStatus--id--get` | GET `/supportCaseStatus/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--supportCaseStatus--id--patch` | PATCH `/supportCaseStatus/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--supportCaseStatus--id--put` | PUT `/supportCaseStatus/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [supportCaseStatus schemas](../schemas/supportCaseStatus.md).

| Definition | Role |
| --- | --- |
| [`supportCaseStatus`](../schemas/supportCaseStatus.md#supportcasestatus) | record body |
| [`supportCaseStatusCollection`](../schemas/supportCaseStatus.md#supportcasestatuscollection) | collection page |
| [`supportCaseStatusSelectOptions`](../schemas/supportCaseStatus.md#supportcasestatusselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
