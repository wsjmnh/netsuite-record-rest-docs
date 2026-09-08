# manufacturingOperationTask

Browser tag `manufacturingOperationTask` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/manufacturingOperationTask`, instance `/manufacturingOperationTask/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/manufacturingOperationTask` | `operation--manufacturingOperationTask-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/manufacturingOperationTask` | `operation--manufacturingOperationTask-get` | Get list of records. |  | 200 OK → `manufacturingOperationTaskCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/manufacturingOperationTask` | `operation--manufacturingOperationTask-patch` | Update records. | `manufacturingOperationTaskCollection` | 202 Accepted; default → `nsError` |
| POST | `/manufacturingOperationTask` | `operation--manufacturingOperationTask-post` | Insert record. | `manufacturingOperationTask` | 200 OK → `manufacturingOperationTask`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/manufacturingOperationTask` | `operation--manufacturingOperationTask-put` | Insert or update records. | `manufacturingOperationTaskCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/manufacturingOperationTask/{id}` | `operation--manufacturingOperationTask--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/manufacturingOperationTask/{id}` | `operation--manufacturingOperationTask--id--get` | Get record. |  | 200 OK → `manufacturingOperationTask`; 202 Accepted; default → `nsError` |
| PATCH | `/manufacturingOperationTask/{id}` | `operation--manufacturingOperationTask--id--patch` | Update record. | `manufacturingOperationTask` | 200 OK → `manufacturingOperationTask`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/manufacturingOperationTask/{id}` | `operation--manufacturingOperationTask--id--put` | Insert or update record. | `manufacturingOperationTask` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--manufacturingOperationTask-delete` | DELETE `/manufacturingOperationTask` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--manufacturingOperationTask-get` | GET `/manufacturingOperationTask` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--manufacturingOperationTask-patch` | PATCH `/manufacturingOperationTask` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--manufacturingOperationTask-post` | POST `/manufacturingOperationTask` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--manufacturingOperationTask-put` | PUT `/manufacturingOperationTask` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--manufacturingOperationTask--id--delete` | DELETE `/manufacturingOperationTask/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--manufacturingOperationTask--id--get` | GET `/manufacturingOperationTask/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--manufacturingOperationTask--id--patch` | PATCH `/manufacturingOperationTask/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--manufacturingOperationTask--id--put` | PUT `/manufacturingOperationTask/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [manufacturingOperationTask schemas](../schemas/manufacturingOperationTask.md).

| Definition | Role |
| --- | --- |
| [`manufacturingOperationTask`](../schemas/manufacturingOperationTask.md#manufacturingoperationtask) | record body |
| [`manufacturingOperationTask-costDetailCollection`](../schemas/manufacturingOperationTask.md#manufacturingoperationtask-costdetailcollection) | sublist/collection |
| [`manufacturingOperationTask-costDetailElement`](../schemas/manufacturingOperationTask.md#manufacturingoperationtask-costdetailelement) | sublist/element |
| [`manufacturingOperationTask-predecessorCollection`](../schemas/manufacturingOperationTask.md#manufacturingoperationtask-predecessorcollection) | sublist/collection |
| [`manufacturingOperationTask-predecessorElement`](../schemas/manufacturingOperationTask.md#manufacturingoperationtask-predecessorelement) | sublist/element |
| [`manufacturingOperationTaskCollection`](../schemas/manufacturingOperationTask.md#manufacturingoperationtaskcollection) | collection page |
| [`manufacturingOperationTaskSelectOptions`](../schemas/manufacturingOperationTask.md#manufacturingoperationtaskselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `costDetail` | [`manufacturingOperationTask-costDetailCollection`](../schemas/manufacturingOperationTask.md#manufacturingoperationtask-costdetailcollection) | [`manufacturingOperationTask-costDetailElement`](../schemas/manufacturingOperationTask.md#manufacturingoperationtask-costdetailelement) |
| `predecessor` | [`manufacturingOperationTask-predecessorCollection`](../schemas/manufacturingOperationTask.md#manufacturingoperationtask-predecessorcollection) | [`manufacturingOperationTask-predecessorElement`](../schemas/manufacturingOperationTask.md#manufacturingoperationtask-predecessorelement) |
