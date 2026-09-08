# partnerCategory

Browser tag `partnerCategory` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/partnerCategory`, instance `/partnerCategory/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/partnerCategory` | `operation--partnerCategory-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/partnerCategory` | `operation--partnerCategory-get` | Get list of records. |  | 200 OK → `partnerCategoryCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/partnerCategory` | `operation--partnerCategory-patch` | Update records. | `partnerCategoryCollection` | 202 Accepted; default → `nsError` |
| POST | `/partnerCategory` | `operation--partnerCategory-post` | Insert record. | `partnerCategory` | 200 OK → `partnerCategory`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/partnerCategory` | `operation--partnerCategory-put` | Insert or update records. | `partnerCategoryCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/partnerCategory/{id}` | `operation--partnerCategory--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/partnerCategory/{id}` | `operation--partnerCategory--id--get` | Get record. |  | 200 OK → `partnerCategory`; 202 Accepted; default → `nsError` |
| PATCH | `/partnerCategory/{id}` | `operation--partnerCategory--id--patch` | Update record. | `partnerCategory` | 200 OK → `partnerCategory`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/partnerCategory/{id}` | `operation--partnerCategory--id--put` | Insert or update record. | `partnerCategory` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--partnerCategory-delete` | DELETE `/partnerCategory` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--partnerCategory-get` | GET `/partnerCategory` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--partnerCategory-patch` | PATCH `/partnerCategory` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--partnerCategory-post` | POST `/partnerCategory` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--partnerCategory-put` | PUT `/partnerCategory` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--partnerCategory--id--delete` | DELETE `/partnerCategory/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--partnerCategory--id--get` | GET `/partnerCategory/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--partnerCategory--id--patch` | PATCH `/partnerCategory/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--partnerCategory--id--put` | PUT `/partnerCategory/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [partnerCategory schemas](../schemas/partnerCategory.md).

| Definition | Role |
| --- | --- |
| [`partnerCategory`](../schemas/partnerCategory.md#partnercategory) | record body |
| [`partnerCategoryCollection`](../schemas/partnerCategory.md#partnercategorycollection) | collection page |
| [`partnerCategorySelectOptions`](../schemas/partnerCategory.md#partnercategoryselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
