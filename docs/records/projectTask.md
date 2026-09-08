# projectTask

Browser tag `projectTask` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/projectTask`, instance `/projectTask/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/projectTask` | `operation--projectTask-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/projectTask` | `operation--projectTask-get` | Get list of records. |  | 200 OK → `projectTaskCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/projectTask` | `operation--projectTask-patch` | Update records. | `projectTaskCollection` | 202 Accepted; default → `nsError` |
| POST | `/projectTask` | `operation--projectTask-post` | Insert record. | `projectTask` | 200 OK → `projectTask`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/projectTask` | `operation--projectTask-put` | Insert or update records. | `projectTaskCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/projectTask/{id}` | `operation--projectTask--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/projectTask/{id}` | `operation--projectTask--id--get` | Get record. |  | 200 OK → `projectTask`; 202 Accepted; default → `nsError` |
| PATCH | `/projectTask/{id}` | `operation--projectTask--id--patch` | Update record. | `projectTask` | 200 OK → `projectTask`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/projectTask/{id}` | `operation--projectTask--id--put` | Insert or update record. | `projectTask` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--projectTask-delete` | DELETE `/projectTask` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--projectTask-get` | GET `/projectTask` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--projectTask-patch` | PATCH `/projectTask` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--projectTask-post` | POST `/projectTask` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--projectTask-put` | PUT `/projectTask` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--projectTask--id--delete` | DELETE `/projectTask/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--projectTask--id--get` | GET `/projectTask/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--projectTask--id--patch` | PATCH `/projectTask/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--projectTask--id--put` | PUT `/projectTask/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [projectTask schemas](../schemas/projectTask.md).

| Definition | Role |
| --- | --- |
| [`projectTask`](../schemas/projectTask.md#projecttask) | record body |
| [`projectTask-assigneeCollection`](../schemas/projectTask.md#projecttask-assigneecollection) | sublist/collection |
| [`projectTask-assigneeElement`](../schemas/projectTask.md#projecttask-assigneeelement) | sublist/element |
| [`projectTask-predecessorCollection`](../schemas/projectTask.md#projecttask-predecessorcollection) | sublist/collection |
| [`projectTask-predecessorElement`](../schemas/projectTask.md#projecttask-predecessorelement) | sublist/element |
| [`projectTaskCollection`](../schemas/projectTask.md#projecttaskcollection) | collection page |
| [`projectTaskSelectOptions`](../schemas/projectTask.md#projecttaskselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `assignee` | [`projectTask-assigneeCollection`](../schemas/projectTask.md#projecttask-assigneecollection) | [`projectTask-assigneeElement`](../schemas/projectTask.md#projecttask-assigneeelement) |
| `predecessor` | [`projectTask-predecessorCollection`](../schemas/projectTask.md#projecttask-predecessorcollection) | [`projectTask-predecessorElement`](../schemas/projectTask.md#projecttask-predecessorelement) |
