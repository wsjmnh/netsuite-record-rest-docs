# budgetimport

Browser tag `budgetimport` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/budgetimport`, instance `/budgetimport/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/budgetimport` | `operation--budgetimport-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/budgetimport` | `operation--budgetimport-get` | Get list of records. |  | 200 OK → `budgetimportCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/budgetimport` | `operation--budgetimport-patch` | Update records. | `budgetimportCollection` | 202 Accepted; default → `nsError` |
| POST | `/budgetimport` | `operation--budgetimport-post` | Insert record. | `budgetimport` | 200 OK → `budgetimport`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/budgetimport` | `operation--budgetimport-put` | Insert or update records. | `budgetimportCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/budgetimport/{id}` | `operation--budgetimport--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/budgetimport/{id}` | `operation--budgetimport--id--get` | Get record. |  | 200 OK → `budgetimport`; 202 Accepted; default → `nsError` |
| PATCH | `/budgetimport/{id}` | `operation--budgetimport--id--patch` | Update record. | `budgetimport` | 200 OK → `budgetimport`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/budgetimport/{id}` | `operation--budgetimport--id--put` | Insert or update record. | `budgetimport` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--budgetimport-delete` | DELETE `/budgetimport` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--budgetimport-get` | GET `/budgetimport` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--budgetimport-patch` | PATCH `/budgetimport` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--budgetimport-post` | POST `/budgetimport` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--budgetimport-put` | PUT `/budgetimport` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--budgetimport--id--delete` | DELETE `/budgetimport/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--budgetimport--id--get` | GET `/budgetimport/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--budgetimport--id--patch` | PATCH `/budgetimport/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--budgetimport--id--put` | PUT `/budgetimport/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [budgetimport schemas](../schemas/budgetimport.md).

| Definition | Role |
| --- | --- |
| [`budgetimport`](../schemas/budgetimport.md#budgetimport) | record body |
| [`budgetimportCollection`](../schemas/budgetimport.md#budgetimportcollection) | collection page |
| [`budgetimportSelectOptions`](../schemas/budgetimport.md#budgetimportselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
