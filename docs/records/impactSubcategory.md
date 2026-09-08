# impactSubcategory

Browser tag `impactSubcategory` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/impactSubcategory`, instance `/impactSubcategory/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/impactSubcategory` | `operation--impactSubcategory-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/impactSubcategory` | `operation--impactSubcategory-get` | Get list of records. |  | 200 OK → `impactSubcategoryCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/impactSubcategory` | `operation--impactSubcategory-patch` | Update records. | `impactSubcategoryCollection` | 202 Accepted; default → `nsError` |
| POST | `/impactSubcategory` | `operation--impactSubcategory-post` | Insert record. | `impactSubcategory` | 200 OK → `impactSubcategory`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/impactSubcategory` | `operation--impactSubcategory-put` | Insert or update records. | `impactSubcategoryCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/impactSubcategory/{id}` | `operation--impactSubcategory--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/impactSubcategory/{id}` | `operation--impactSubcategory--id--get` | Get record. |  | 200 OK → `impactSubcategory`; 202 Accepted; default → `nsError` |
| PATCH | `/impactSubcategory/{id}` | `operation--impactSubcategory--id--patch` | Update record. | `impactSubcategory` | 200 OK → `impactSubcategory`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/impactSubcategory/{id}` | `operation--impactSubcategory--id--put` | Insert or update record. | `impactSubcategory` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--impactSubcategory-delete` | DELETE `/impactSubcategory` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--impactSubcategory-get` | GET `/impactSubcategory` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--impactSubcategory-patch` | PATCH `/impactSubcategory` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--impactSubcategory-post` | POST `/impactSubcategory` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--impactSubcategory-put` | PUT `/impactSubcategory` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--impactSubcategory--id--delete` | DELETE `/impactSubcategory/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--impactSubcategory--id--get` | GET `/impactSubcategory/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--impactSubcategory--id--patch` | PATCH `/impactSubcategory/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--impactSubcategory--id--put` | PUT `/impactSubcategory/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [impactSubcategory schemas](../schemas/impactSubcategory.md).

| Definition | Role |
| --- | --- |
| [`impactSubcategory`](../schemas/impactSubcategory.md#impactsubcategory) | record body |
| [`impactSubcategoryCollection`](../schemas/impactSubcategory.md#impactsubcategorycollection) | collection page |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
