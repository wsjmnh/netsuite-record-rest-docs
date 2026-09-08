# automatedClearingHouse

Browser tag `automatedClearingHouse` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/automatedClearingHouse`, instance `/automatedClearingHouse/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/automatedClearingHouse` | `operation--automatedClearingHouse-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/automatedClearingHouse` | `operation--automatedClearingHouse-get` | Get list of records. |  | 200 OK → `automatedClearingHouseCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/automatedClearingHouse` | `operation--automatedClearingHouse-patch` | Update records. | `automatedClearingHouseCollection` | 202 Accepted; default → `nsError` |
| POST | `/automatedClearingHouse` | `operation--automatedClearingHouse-post` | Insert record. | `automatedClearingHouse` | 200 OK → `automatedClearingHouse`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/automatedClearingHouse` | `operation--automatedClearingHouse-put` | Insert or update records. | `automatedClearingHouseCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/automatedClearingHouse/{id}` | `operation--automatedClearingHouse--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/automatedClearingHouse/{id}` | `operation--automatedClearingHouse--id--get` | Get record. |  | 200 OK → `automatedClearingHouse`; 202 Accepted; default → `nsError` |
| PATCH | `/automatedClearingHouse/{id}` | `operation--automatedClearingHouse--id--patch` | Update record. | `automatedClearingHouse` | 200 OK → `automatedClearingHouse`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/automatedClearingHouse/{id}` | `operation--automatedClearingHouse--id--put` | Insert or update record. | `automatedClearingHouse` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--automatedClearingHouse-delete` | DELETE `/automatedClearingHouse` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--automatedClearingHouse-get` | GET `/automatedClearingHouse` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--automatedClearingHouse-patch` | PATCH `/automatedClearingHouse` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--automatedClearingHouse-post` | POST `/automatedClearingHouse` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--automatedClearingHouse-put` | PUT `/automatedClearingHouse` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--automatedClearingHouse--id--delete` | DELETE `/automatedClearingHouse/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--automatedClearingHouse--id--get` | GET `/automatedClearingHouse/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--automatedClearingHouse--id--patch` | PATCH `/automatedClearingHouse/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--automatedClearingHouse--id--put` | PUT `/automatedClearingHouse/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [automatedClearingHouse schemas](../schemas/automatedClearingHouse.md).

| Definition | Role |
| --- | --- |
| [`automatedClearingHouse`](../schemas/automatedClearingHouse.md#automatedclearinghouse) | record body |
| [`automatedClearingHouseCollection`](../schemas/automatedClearingHouse.md#automatedclearinghousecollection) | collection page |
| [`automatedClearingHouseSelectOptions`](../schemas/automatedClearingHouse.md#automatedclearinghouseselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
