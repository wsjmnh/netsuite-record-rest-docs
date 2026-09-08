# customerStatus

Browser tag `customerStatus` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/customerStatus`, instance `/customerStatus/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/customerStatus` | `operation--customerStatus-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/customerStatus` | `operation--customerStatus-get` | Get list of records. |  | 200 OK → `customerStatusCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/customerStatus` | `operation--customerStatus-patch` | Update records. | `customerStatusCollection` | 202 Accepted; default → `nsError` |
| POST | `/customerStatus` | `operation--customerStatus-post` | Insert record. | `customerStatus` | 200 OK → `customerStatus`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/customerStatus` | `operation--customerStatus-put` | Insert or update records. | `customerStatusCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/customerStatus/{id}` | `operation--customerStatus--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/customerStatus/{id}` | `operation--customerStatus--id--get` | Get record. |  | 200 OK → `customerStatus`; 202 Accepted; default → `nsError` |
| PATCH | `/customerStatus/{id}` | `operation--customerStatus--id--patch` | Update record. | `customerStatus` | 200 OK → `customerStatus`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/customerStatus/{id}` | `operation--customerStatus--id--put` | Insert or update record. | `customerStatus` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--customerStatus-delete` | DELETE `/customerStatus` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerStatus-get` | GET `/customerStatus` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerStatus-patch` | PATCH `/customerStatus` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerStatus-post` | POST `/customerStatus` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--customerStatus-put` | PUT `/customerStatus` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerStatus--id--delete` | DELETE `/customerStatus/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerStatus--id--get` | GET `/customerStatus/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerStatus--id--patch` | PATCH `/customerStatus/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--customerStatus--id--put` | PUT `/customerStatus/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [customerStatus schemas](../schemas/customerStatus.md).

| Definition | Role |
| --- | --- |
| [`customerStatus`](../schemas/customerStatus.md#customerstatus) | record body |
| [`customerStatusCollection`](../schemas/customerStatus.md#customerstatuscollection) | collection page |
| [`customerStatusSelectOptions`](../schemas/customerStatus.md#customerstatusselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
