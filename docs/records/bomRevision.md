# bomRevision

Browser tag `bomRevision` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/bomRevision`, instance `/bomRevision/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/bomRevision` | `operation--bomRevision-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/bomRevision` | `operation--bomRevision-get` | Get list of records. |  | 200 OK → `bomRevisionCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/bomRevision` | `operation--bomRevision-patch` | Update records. | `bomRevisionCollection` | 202 Accepted; default → `nsError` |
| POST | `/bomRevision` | `operation--bomRevision-post` | Insert record. | `bomRevision` | 200 OK → `bomRevision`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/bomRevision` | `operation--bomRevision-put` | Insert or update records. | `bomRevisionCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/bomRevision/{id}` | `operation--bomRevision--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/bomRevision/{id}` | `operation--bomRevision--id--get` | Get record. |  | 200 OK → `bomRevision`; 202 Accepted; default → `nsError` |
| PATCH | `/bomRevision/{id}` | `operation--bomRevision--id--patch` | Update record. | `bomRevision` | 200 OK → `bomRevision`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/bomRevision/{id}` | `operation--bomRevision--id--put` | Insert or update record. | `bomRevision` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--bomRevision-delete` | DELETE `/bomRevision` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--bomRevision-get` | GET `/bomRevision` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--bomRevision-patch` | PATCH `/bomRevision` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--bomRevision-post` | POST `/bomRevision` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--bomRevision-put` | PUT `/bomRevision` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--bomRevision--id--delete` | DELETE `/bomRevision/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--bomRevision--id--get` | GET `/bomRevision/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--bomRevision--id--patch` | PATCH `/bomRevision/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--bomRevision--id--put` | PUT `/bomRevision/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [bomRevision schemas](../schemas/bomRevision.md).

| Definition | Role |
| --- | --- |
| [`bomRevision`](../schemas/bomRevision.md#bomrevision) | record body |
| [`bomRevision-componentCollection`](../schemas/bomRevision.md#bomrevision-componentcollection) | sublist/collection |
| [`bomRevision-componentElement`](../schemas/bomRevision.md#bomrevision-componentelement) | sublist/element |
| [`bomRevisionCollection`](../schemas/bomRevision.md#bomrevisioncollection) | collection page |
| [`bomRevisionSelectOptions`](../schemas/bomRevision.md#bomrevisionselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `component` | [`bomRevision-componentCollection`](../schemas/bomRevision.md#bomrevision-componentcollection) | [`bomRevision-componentElement`](../schemas/bomRevision.md#bomrevision-componentelement) |
