# merchandiseHierarchyLevel

Browser tag `merchandiseHierarchyLevel` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/merchandiseHierarchyLevel`, instance `/merchandiseHierarchyLevel/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/merchandiseHierarchyLevel` | `operation--merchandiseHierarchyLevel-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/merchandiseHierarchyLevel` | `operation--merchandiseHierarchyLevel-get` | Get list of records. |  | 200 OK → `merchandiseHierarchyLevelCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/merchandiseHierarchyLevel` | `operation--merchandiseHierarchyLevel-patch` | Update records. | `merchandiseHierarchyLevelCollection` | 202 Accepted; default → `nsError` |
| POST | `/merchandiseHierarchyLevel` | `operation--merchandiseHierarchyLevel-post` | Insert record. | `merchandiseHierarchyLevel` | 200 OK → `merchandiseHierarchyLevel`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/merchandiseHierarchyLevel` | `operation--merchandiseHierarchyLevel-put` | Insert or update records. | `merchandiseHierarchyLevelCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/merchandiseHierarchyLevel/{id}` | `operation--merchandiseHierarchyLevel--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/merchandiseHierarchyLevel/{id}` | `operation--merchandiseHierarchyLevel--id--get` | Get record. |  | 200 OK → `merchandiseHierarchyLevel`; 202 Accepted; default → `nsError` |
| PATCH | `/merchandiseHierarchyLevel/{id}` | `operation--merchandiseHierarchyLevel--id--patch` | Update record. | `merchandiseHierarchyLevel` | 200 OK → `merchandiseHierarchyLevel`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/merchandiseHierarchyLevel/{id}` | `operation--merchandiseHierarchyLevel--id--put` | Insert or update record. | `merchandiseHierarchyLevel` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--merchandiseHierarchyLevel-delete` | DELETE `/merchandiseHierarchyLevel` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--merchandiseHierarchyLevel-get` | GET `/merchandiseHierarchyLevel` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--merchandiseHierarchyLevel-patch` | PATCH `/merchandiseHierarchyLevel` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--merchandiseHierarchyLevel-post` | POST `/merchandiseHierarchyLevel` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--merchandiseHierarchyLevel-put` | PUT `/merchandiseHierarchyLevel` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--merchandiseHierarchyLevel--id--delete` | DELETE `/merchandiseHierarchyLevel/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--merchandiseHierarchyLevel--id--get` | GET `/merchandiseHierarchyLevel/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--merchandiseHierarchyLevel--id--patch` | PATCH `/merchandiseHierarchyLevel/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--merchandiseHierarchyLevel--id--put` | PUT `/merchandiseHierarchyLevel/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [merchandiseHierarchyLevel schemas](../schemas/merchandiseHierarchyLevel.md).

| Definition | Role |
| --- | --- |
| [`merchandiseHierarchyLevel`](../schemas/merchandiseHierarchyLevel.md#merchandisehierarchylevel) | record body |
| [`merchandiseHierarchyLevelCollection`](../schemas/merchandiseHierarchyLevel.md#merchandisehierarchylevelcollection) | collection page |
| [`merchandiseHierarchyLevelSelectOptions`](../schemas/merchandiseHierarchyLevel.md#merchandisehierarchylevelselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
