# itemRevision

Browser tag `itemRevision` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/itemRevision`, instance `/itemRevision/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/itemRevision` | `operation--itemRevision-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/itemRevision` | `operation--itemRevision-get` | Get list of records. |  | 200 OK → `itemRevisionCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/itemRevision` | `operation--itemRevision-patch` | Update records. | `itemRevisionCollection` | 202 Accepted; default → `nsError` |
| POST | `/itemRevision` | `operation--itemRevision-post` | Insert record. | `itemRevision` | 200 OK → `itemRevision`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/itemRevision` | `operation--itemRevision-put` | Insert or update records. | `itemRevisionCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/itemRevision/{id}` | `operation--itemRevision--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/itemRevision/{id}` | `operation--itemRevision--id--get` | Get record. |  | 200 OK → `itemRevision`; 202 Accepted; default → `nsError` |
| PATCH | `/itemRevision/{id}` | `operation--itemRevision--id--patch` | Update record. | `itemRevision` | 200 OK → `itemRevision`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/itemRevision/{id}` | `operation--itemRevision--id--put` | Insert or update record. | `itemRevision` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--itemRevision-delete` | DELETE `/itemRevision` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemRevision-get` | GET `/itemRevision` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemRevision-patch` | PATCH `/itemRevision` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemRevision-post` | POST `/itemRevision` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--itemRevision-put` | PUT `/itemRevision` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemRevision--id--delete` | DELETE `/itemRevision/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemRevision--id--get` | GET `/itemRevision/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemRevision--id--patch` | PATCH `/itemRevision/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--itemRevision--id--put` | PUT `/itemRevision/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [itemRevision schemas](../schemas/itemRevision.md).

| Definition | Role |
| --- | --- |
| [`itemRevision`](../schemas/itemRevision.md#itemrevision) | record body |
| [`itemRevisionCollection`](../schemas/itemRevision.md#itemrevisioncollection) | collection page |
| [`itemRevisionSelectOptions`](../schemas/itemRevision.md#itemrevisionselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
