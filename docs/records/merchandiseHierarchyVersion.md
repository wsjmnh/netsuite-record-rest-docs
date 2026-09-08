# merchandiseHierarchyVersion

Browser tag `merchandiseHierarchyVersion` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/merchandiseHierarchyVersion`, instance `/merchandiseHierarchyVersion/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/merchandiseHierarchyVersion` | `operation--merchandiseHierarchyVersion-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/merchandiseHierarchyVersion` | `operation--merchandiseHierarchyVersion-get` | Get list of records. |  | 200 OK → `merchandiseHierarchyVersionCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/merchandiseHierarchyVersion` | `operation--merchandiseHierarchyVersion-patch` | Update records. | `merchandiseHierarchyVersionCollection` | 202 Accepted; default → `nsError` |
| POST | `/merchandiseHierarchyVersion` | `operation--merchandiseHierarchyVersion-post` | Insert record. | `merchandiseHierarchyVersion` | 200 OK → `merchandiseHierarchyVersion`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/merchandiseHierarchyVersion` | `operation--merchandiseHierarchyVersion-put` | Insert or update records. | `merchandiseHierarchyVersionCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/merchandiseHierarchyVersion/{id}` | `operation--merchandiseHierarchyVersion--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/merchandiseHierarchyVersion/{id}` | `operation--merchandiseHierarchyVersion--id--get` | Get record. |  | 200 OK → `merchandiseHierarchyVersion`; 202 Accepted; default → `nsError` |
| PATCH | `/merchandiseHierarchyVersion/{id}` | `operation--merchandiseHierarchyVersion--id--patch` | Update record. | `merchandiseHierarchyVersion` | 200 OK → `merchandiseHierarchyVersion`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/merchandiseHierarchyVersion/{id}` | `operation--merchandiseHierarchyVersion--id--put` | Insert or update record. | `merchandiseHierarchyVersion` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--merchandiseHierarchyVersion-delete` | DELETE `/merchandiseHierarchyVersion` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--merchandiseHierarchyVersion-get` | GET `/merchandiseHierarchyVersion` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--merchandiseHierarchyVersion-patch` | PATCH `/merchandiseHierarchyVersion` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--merchandiseHierarchyVersion-post` | POST `/merchandiseHierarchyVersion` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--merchandiseHierarchyVersion-put` | PUT `/merchandiseHierarchyVersion` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--merchandiseHierarchyVersion--id--delete` | DELETE `/merchandiseHierarchyVersion/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--merchandiseHierarchyVersion--id--get` | GET `/merchandiseHierarchyVersion/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--merchandiseHierarchyVersion--id--patch` | PATCH `/merchandiseHierarchyVersion/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--merchandiseHierarchyVersion--id--put` | PUT `/merchandiseHierarchyVersion/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [merchandiseHierarchyVersion schemas](../schemas/merchandiseHierarchyVersion.md).

| Definition | Role |
| --- | --- |
| [`merchandiseHierarchyVersion`](../schemas/merchandiseHierarchyVersion.md#merchandisehierarchyversion) | record body |
| [`merchandiseHierarchyVersion-hierarchylevelsCollection`](../schemas/merchandiseHierarchyVersion.md#merchandisehierarchyversion-hierarchylevelscollection) | sublist/collection |
| [`merchandiseHierarchyVersion-hierarchylevelsElement`](../schemas/merchandiseHierarchyVersion.md#merchandisehierarchyversion-hierarchylevelselement) | sublist/element |
| [`merchandiseHierarchyVersionCollection`](../schemas/merchandiseHierarchyVersion.md#merchandisehierarchyversioncollection) | collection page |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `hierarchylevels` | [`merchandiseHierarchyVersion-hierarchylevelsCollection`](../schemas/merchandiseHierarchyVersion.md#merchandisehierarchyversion-hierarchylevelscollection) | [`merchandiseHierarchyVersion-hierarchylevelsElement`](../schemas/merchandiseHierarchyVersion.md#merchandisehierarchyversion-hierarchylevelselement) |
