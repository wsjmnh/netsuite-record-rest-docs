# supportCasePriority

Browser tag `supportCasePriority` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/supportCasePriority`, instance `/supportCasePriority/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/supportCasePriority` | `operation--supportCasePriority-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/supportCasePriority` | `operation--supportCasePriority-get` | Get list of records. |  | 200 OK → `supportCasePriorityCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/supportCasePriority` | `operation--supportCasePriority-patch` | Update records. | `supportCasePriorityCollection` | 202 Accepted; default → `nsError` |
| POST | `/supportCasePriority` | `operation--supportCasePriority-post` | Insert record. | `supportCasePriority` | 200 OK → `supportCasePriority`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/supportCasePriority` | `operation--supportCasePriority-put` | Insert or update records. | `supportCasePriorityCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/supportCasePriority/{id}` | `operation--supportCasePriority--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/supportCasePriority/{id}` | `operation--supportCasePriority--id--get` | Get record. |  | 200 OK → `supportCasePriority`; 202 Accepted; default → `nsError` |
| PATCH | `/supportCasePriority/{id}` | `operation--supportCasePriority--id--patch` | Update record. | `supportCasePriority` | 200 OK → `supportCasePriority`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/supportCasePriority/{id}` | `operation--supportCasePriority--id--put` | Insert or update record. | `supportCasePriority` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--supportCasePriority-delete` | DELETE `/supportCasePriority` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--supportCasePriority-get` | GET `/supportCasePriority` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--supportCasePriority-patch` | PATCH `/supportCasePriority` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--supportCasePriority-post` | POST `/supportCasePriority` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--supportCasePriority-put` | PUT `/supportCasePriority` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--supportCasePriority--id--delete` | DELETE `/supportCasePriority/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--supportCasePriority--id--get` | GET `/supportCasePriority/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--supportCasePriority--id--patch` | PATCH `/supportCasePriority/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--supportCasePriority--id--put` | PUT `/supportCasePriority/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [supportCasePriority schemas](../schemas/supportCasePriority.md).

| Definition | Role |
| --- | --- |
| [`supportCasePriority`](../schemas/supportCasePriority.md#supportcasepriority) | record body |
| [`supportCasePriorityCollection`](../schemas/supportCasePriority.md#supportcaseprioritycollection) | collection page |
| [`supportCasePrioritySelectOptions`](../schemas/supportCasePriority.md#supportcasepriorityselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
