# salesRole

Browser tag `salesRole` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/salesRole`, instance `/salesRole/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/salesRole` | `operation--salesRole-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/salesRole` | `operation--salesRole-get` | Get list of records. |  | 200 OK → `salesRoleCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/salesRole` | `operation--salesRole-patch` | Update records. | `salesRoleCollection` | 202 Accepted; default → `nsError` |
| POST | `/salesRole` | `operation--salesRole-post` | Insert record. | `salesRole` | 200 OK → `salesRole`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/salesRole` | `operation--salesRole-put` | Insert or update records. | `salesRoleCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/salesRole/{id}` | `operation--salesRole--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/salesRole/{id}` | `operation--salesRole--id--get` | Get record. |  | 200 OK → `salesRole`; 202 Accepted; default → `nsError` |
| PATCH | `/salesRole/{id}` | `operation--salesRole--id--patch` | Update record. | `salesRole` | 200 OK → `salesRole`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/salesRole/{id}` | `operation--salesRole--id--put` | Insert or update record. | `salesRole` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--salesRole-delete` | DELETE `/salesRole` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--salesRole-get` | GET `/salesRole` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--salesRole-patch` | PATCH `/salesRole` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--salesRole-post` | POST `/salesRole` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--salesRole-put` | PUT `/salesRole` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--salesRole--id--delete` | DELETE `/salesRole/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--salesRole--id--get` | GET `/salesRole/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--salesRole--id--patch` | PATCH `/salesRole/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--salesRole--id--put` | PUT `/salesRole/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [salesRole schemas](../schemas/salesRole.md).

| Definition | Role |
| --- | --- |
| [`salesRole`](../schemas/salesRole.md#salesrole) | record body |
| [`salesRoleCollection`](../schemas/salesRole.md#salesrolecollection) | collection page |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
