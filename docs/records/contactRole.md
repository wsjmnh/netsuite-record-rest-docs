# contactRole

Browser tag `contactRole` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/contactRole`, instance `/contactRole/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/contactRole` | `operation--contactRole-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/contactRole` | `operation--contactRole-get` | Get list of records. |  | 200 OK → `contactRoleCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/contactRole` | `operation--contactRole-patch` | Update records. | `contactRoleCollection` | 202 Accepted; default → `nsError` |
| POST | `/contactRole` | `operation--contactRole-post` | Insert record. | `contactRole` | 200 OK → `contactRole`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/contactRole` | `operation--contactRole-put` | Insert or update records. | `contactRoleCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/contactRole/{id}` | `operation--contactRole--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/contactRole/{id}` | `operation--contactRole--id--get` | Get record. |  | 200 OK → `contactRole`; 202 Accepted; default → `nsError` |
| PATCH | `/contactRole/{id}` | `operation--contactRole--id--patch` | Update record. | `contactRole` | 200 OK → `contactRole`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/contactRole/{id}` | `operation--contactRole--id--put` | Insert or update record. | `contactRole` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--contactRole-delete` | DELETE `/contactRole` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--contactRole-get` | GET `/contactRole` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--contactRole-patch` | PATCH `/contactRole` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--contactRole-post` | POST `/contactRole` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--contactRole-put` | PUT `/contactRole` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--contactRole--id--delete` | DELETE `/contactRole/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--contactRole--id--get` | GET `/contactRole/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--contactRole--id--patch` | PATCH `/contactRole/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--contactRole--id--put` | PUT `/contactRole/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [contactRole schemas](../schemas/contactRole.md).

| Definition | Role |
| --- | --- |
| [`contactRole`](../schemas/contactRole.md#contactrole) | record body |
| [`contactRoleCollection`](../schemas/contactRole.md#contactrolecollection) | collection page |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
