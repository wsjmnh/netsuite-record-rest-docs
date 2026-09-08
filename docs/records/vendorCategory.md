# vendorCategory

Browser tag `vendorCategory` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/vendorCategory`, instance `/vendorCategory/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/vendorCategory` | `operation--vendorCategory-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/vendorCategory` | `operation--vendorCategory-get` | Get list of records. |  | 200 OK → `vendorCategoryCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/vendorCategory` | `operation--vendorCategory-patch` | Update records. | `vendorCategoryCollection` | 202 Accepted; default → `nsError` |
| POST | `/vendorCategory` | `operation--vendorCategory-post` | Insert record. | `vendorCategory` | 200 OK → `vendorCategory`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/vendorCategory` | `operation--vendorCategory-put` | Insert or update records. | `vendorCategoryCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/vendorCategory/{id}` | `operation--vendorCategory--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/vendorCategory/{id}` | `operation--vendorCategory--id--get` | Get record. |  | 200 OK → `vendorCategory`; 202 Accepted; default → `nsError` |
| PATCH | `/vendorCategory/{id}` | `operation--vendorCategory--id--patch` | Update record. | `vendorCategory` | 200 OK → `vendorCategory`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/vendorCategory/{id}` | `operation--vendorCategory--id--put` | Insert or update record. | `vendorCategory` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--vendorCategory-delete` | DELETE `/vendorCategory` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorCategory-get` | GET `/vendorCategory` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorCategory-patch` | PATCH `/vendorCategory` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorCategory-post` | POST `/vendorCategory` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--vendorCategory-put` | PUT `/vendorCategory` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorCategory--id--delete` | DELETE `/vendorCategory/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorCategory--id--get` | GET `/vendorCategory/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorCategory--id--patch` | PATCH `/vendorCategory/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--vendorCategory--id--put` | PUT `/vendorCategory/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [vendorCategory schemas](../schemas/vendorCategory.md).

| Definition | Role |
| --- | --- |
| [`vendorCategory`](../schemas/vendorCategory.md#vendorcategory) | record body |
| [`vendorCategoryCollection`](../schemas/vendorCategory.md#vendorcategorycollection) | collection page |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
