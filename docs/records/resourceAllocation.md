# resourceAllocation

Browser tag `resourceAllocation` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/resourceAllocation`, instance `/resourceAllocation/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/resourceAllocation` | `operation--resourceAllocation-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/resourceAllocation` | `operation--resourceAllocation-get` | Get list of records. |  | 200 OK → `resourceAllocationCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/resourceAllocation` | `operation--resourceAllocation-patch` | Update records. | `resourceAllocationCollection` | 202 Accepted; default → `nsError` |
| POST | `/resourceAllocation` | `operation--resourceAllocation-post` | Insert record. | `resourceAllocation` | 200 OK → `resourceAllocation`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/resourceAllocation` | `operation--resourceAllocation-put` | Insert or update records. | `resourceAllocationCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/resourceAllocation/{id}` | `operation--resourceAllocation--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/resourceAllocation/{id}` | `operation--resourceAllocation--id--get` | Get record. |  | 200 OK → `resourceAllocation`; 202 Accepted; default → `nsError` |
| PATCH | `/resourceAllocation/{id}` | `operation--resourceAllocation--id--patch` | Update record. | `resourceAllocation` | 200 OK → `resourceAllocation`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/resourceAllocation/{id}` | `operation--resourceAllocation--id--put` | Insert or update record. | `resourceAllocation` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--resourceAllocation-delete` | DELETE `/resourceAllocation` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--resourceAllocation-get` | GET `/resourceAllocation` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--resourceAllocation-patch` | PATCH `/resourceAllocation` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--resourceAllocation-post` | POST `/resourceAllocation` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--resourceAllocation-put` | PUT `/resourceAllocation` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--resourceAllocation--id--delete` | DELETE `/resourceAllocation/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--resourceAllocation--id--get` | GET `/resourceAllocation/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--resourceAllocation--id--patch` | PATCH `/resourceAllocation/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--resourceAllocation--id--put` | PUT `/resourceAllocation/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [resourceAllocation schemas](../schemas/resourceAllocation.md).

| Definition | Role |
| --- | --- |
| [`resourceAllocation`](../schemas/resourceAllocation.md#resourceallocation) | record body |
| [`resourceAllocationCollection`](../schemas/resourceAllocation.md#resourceallocationcollection) | collection page |
| [`resourceAllocationSelectOptions`](../schemas/resourceAllocation.md#resourceallocationselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
