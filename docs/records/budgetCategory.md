# budgetCategory

Browser tag `budgetCategory` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/budgetCategory`, instance `/budgetCategory/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/budgetCategory` | `operation--budgetCategory-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/budgetCategory` | `operation--budgetCategory-get` | Get list of records. |  | 200 OK → `budgetCategoryCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/budgetCategory` | `operation--budgetCategory-patch` | Update records. | `budgetCategoryCollection` | 202 Accepted; default → `nsError` |
| POST | `/budgetCategory` | `operation--budgetCategory-post` | Insert record. | `budgetCategory` | 200 OK → `budgetCategory`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/budgetCategory` | `operation--budgetCategory-put` | Insert or update records. | `budgetCategoryCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/budgetCategory/{id}` | `operation--budgetCategory--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/budgetCategory/{id}` | `operation--budgetCategory--id--get` | Get record. |  | 200 OK → `budgetCategory`; 202 Accepted; default → `nsError` |
| PATCH | `/budgetCategory/{id}` | `operation--budgetCategory--id--patch` | Update record. | `budgetCategory` | 200 OK → `budgetCategory`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/budgetCategory/{id}` | `operation--budgetCategory--id--put` | Insert or update record. | `budgetCategory` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--budgetCategory-delete` | DELETE `/budgetCategory` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--budgetCategory-get` | GET `/budgetCategory` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--budgetCategory-patch` | PATCH `/budgetCategory` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--budgetCategory-post` | POST `/budgetCategory` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--budgetCategory-put` | PUT `/budgetCategory` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--budgetCategory--id--delete` | DELETE `/budgetCategory/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--budgetCategory--id--get` | GET `/budgetCategory/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--budgetCategory--id--patch` | PATCH `/budgetCategory/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--budgetCategory--id--put` | PUT `/budgetCategory/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [budgetCategory schemas](../schemas/budgetCategory.md).

| Definition | Role |
| --- | --- |
| [`budgetCategory`](../schemas/budgetCategory.md#budgetcategory) | record body |
| [`budgetCategoryCollection`](../schemas/budgetCategory.md#budgetcategorycollection) | collection page |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
