# otherNameCategory

Browser tag `otherNameCategory` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/otherNameCategory`, instance `/otherNameCategory/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/otherNameCategory` | `operation--otherNameCategory-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/otherNameCategory` | `operation--otherNameCategory-get` | Get list of records. |  | 200 OK → `otherNameCategoryCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/otherNameCategory` | `operation--otherNameCategory-patch` | Update records. | `otherNameCategoryCollection` | 202 Accepted; default → `nsError` |
| POST | `/otherNameCategory` | `operation--otherNameCategory-post` | Insert record. | `otherNameCategory` | 200 OK → `otherNameCategory`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/otherNameCategory` | `operation--otherNameCategory-put` | Insert or update records. | `otherNameCategoryCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/otherNameCategory/{id}` | `operation--otherNameCategory--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/otherNameCategory/{id}` | `operation--otherNameCategory--id--get` | Get record. |  | 200 OK → `otherNameCategory`; 202 Accepted; default → `nsError` |
| PATCH | `/otherNameCategory/{id}` | `operation--otherNameCategory--id--patch` | Update record. | `otherNameCategory` | 200 OK → `otherNameCategory`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/otherNameCategory/{id}` | `operation--otherNameCategory--id--put` | Insert or update record. | `otherNameCategory` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--otherNameCategory-delete` | DELETE `/otherNameCategory` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--otherNameCategory-get` | GET `/otherNameCategory` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--otherNameCategory-patch` | PATCH `/otherNameCategory` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--otherNameCategory-post` | POST `/otherNameCategory` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--otherNameCategory-put` | PUT `/otherNameCategory` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--otherNameCategory--id--delete` | DELETE `/otherNameCategory/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--otherNameCategory--id--get` | GET `/otherNameCategory/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--otherNameCategory--id--patch` | PATCH `/otherNameCategory/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--otherNameCategory--id--put` | PUT `/otherNameCategory/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [otherNameCategory schemas](../schemas/otherNameCategory.md).

| Definition | Role |
| --- | --- |
| [`otherNameCategory`](../schemas/otherNameCategory.md#othernamecategory) | record body |
| [`otherNameCategoryCollection`](../schemas/otherNameCategory.md#othernamecategorycollection) | collection page |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
