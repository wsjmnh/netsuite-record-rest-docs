# merchandiseHierarchyNode

Browser tag `merchandiseHierarchyNode` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/merchandiseHierarchyNode`, instance `/merchandiseHierarchyNode/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/merchandiseHierarchyNode` | `operation--merchandiseHierarchyNode-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/merchandiseHierarchyNode` | `operation--merchandiseHierarchyNode-get` | Get list of records. |  | 200 OK → `merchandiseHierarchyNodeCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/merchandiseHierarchyNode` | `operation--merchandiseHierarchyNode-patch` | Update records. | `merchandiseHierarchyNodeCollection` | 202 Accepted; default → `nsError` |
| POST | `/merchandiseHierarchyNode` | `operation--merchandiseHierarchyNode-post` | Insert record. | `merchandiseHierarchyNode` | 200 OK → `merchandiseHierarchyNode`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/merchandiseHierarchyNode` | `operation--merchandiseHierarchyNode-put` | Insert or update records. | `merchandiseHierarchyNodeCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/merchandiseHierarchyNode/{id}` | `operation--merchandiseHierarchyNode--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/merchandiseHierarchyNode/{id}` | `operation--merchandiseHierarchyNode--id--get` | Get record. |  | 200 OK → `merchandiseHierarchyNode`; 202 Accepted; default → `nsError` |
| PATCH | `/merchandiseHierarchyNode/{id}` | `operation--merchandiseHierarchyNode--id--patch` | Update record. | `merchandiseHierarchyNode` | 200 OK → `merchandiseHierarchyNode`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/merchandiseHierarchyNode/{id}` | `operation--merchandiseHierarchyNode--id--put` | Insert or update record. | `merchandiseHierarchyNode` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--merchandiseHierarchyNode-delete` | DELETE `/merchandiseHierarchyNode` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--merchandiseHierarchyNode-get` | GET `/merchandiseHierarchyNode` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--merchandiseHierarchyNode-patch` | PATCH `/merchandiseHierarchyNode` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--merchandiseHierarchyNode-post` | POST `/merchandiseHierarchyNode` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--merchandiseHierarchyNode-put` | PUT `/merchandiseHierarchyNode` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--merchandiseHierarchyNode--id--delete` | DELETE `/merchandiseHierarchyNode/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--merchandiseHierarchyNode--id--get` | GET `/merchandiseHierarchyNode/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--merchandiseHierarchyNode--id--patch` | PATCH `/merchandiseHierarchyNode/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--merchandiseHierarchyNode--id--put` | PUT `/merchandiseHierarchyNode/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [merchandiseHierarchyNode schemas](../schemas/merchandiseHierarchyNode.md).

| Definition | Role |
| --- | --- |
| [`merchandiseHierarchyNode`](../schemas/merchandiseHierarchyNode.md#merchandisehierarchynode) | record body |
| [`merchandiseHierarchyNode-hierarchyversionsCollection`](../schemas/merchandiseHierarchyNode.md#merchandisehierarchynode-hierarchyversionscollection) | sublist/collection |
| [`merchandiseHierarchyNode-hierarchyversionsElement`](../schemas/merchandiseHierarchyNode.md#merchandisehierarchynode-hierarchyversionselement) | sublist/element |
| [`merchandiseHierarchyNodeCollection`](../schemas/merchandiseHierarchyNode.md#merchandisehierarchynodecollection) | collection page |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `hierarchyversions` | [`merchandiseHierarchyNode-hierarchyversionsCollection`](../schemas/merchandiseHierarchyNode.md#merchandisehierarchynode-hierarchyversionscollection) | [`merchandiseHierarchyNode-hierarchyversionsElement`](../schemas/merchandiseHierarchyNode.md#merchandisehierarchynode-hierarchyversionselement) |
