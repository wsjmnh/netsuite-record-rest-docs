# workOrderClose

Browser tag `workOrderClose` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/workOrderClose`, instance `/workOrderClose/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/workOrderClose` | `operation--workOrderClose-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/workOrderClose` | `operation--workOrderClose-get` | Get list of records. |  | 200 OK → `workOrderCloseCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/workOrderClose` | `operation--workOrderClose-patch` | Update records. | `workOrderCloseCollection` | 202 Accepted; default → `nsError` |
| POST | `/workOrderClose` | `operation--workOrderClose-post` | Insert record. | `workOrderClose` | 200 OK → `workOrderClose`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/workOrderClose` | `operation--workOrderClose-put` | Insert or update records. | `workOrderCloseCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/workOrderClose/{id}` | `operation--workOrderClose--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/workOrderClose/{id}` | `operation--workOrderClose--id--get` | Get record. |  | 200 OK → `workOrderClose`; 202 Accepted; default → `nsError` |
| PATCH | `/workOrderClose/{id}` | `operation--workOrderClose--id--patch` | Update record. | `workOrderClose` | 200 OK → `workOrderClose`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/workOrderClose/{id}` | `operation--workOrderClose--id--put` | Insert or update record. | `workOrderClose` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--workOrderClose-delete` | DELETE `/workOrderClose` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--workOrderClose-get` | GET `/workOrderClose` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--workOrderClose-patch` | PATCH `/workOrderClose` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--workOrderClose-post` | POST `/workOrderClose` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--workOrderClose-put` | PUT `/workOrderClose` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--workOrderClose--id--delete` | DELETE `/workOrderClose/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--workOrderClose--id--get` | GET `/workOrderClose/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--workOrderClose--id--patch` | PATCH `/workOrderClose/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--workOrderClose--id--put` | PUT `/workOrderClose/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [workOrderClose schemas](../schemas/workOrderClose.md).

| Definition | Role |
| --- | --- |
| [`workOrderClose`](../schemas/workOrderClose.md#workorderclose) | record body |
| [`workOrderClose-componentCollection`](../schemas/workOrderClose.md#workorderclose-componentcollection) | sublist/collection |
| [`workOrderClose-componentElement`](../schemas/workOrderClose.md#workorderclose-componentelement) | sublist/element |
| [`workOrderClose-routingItemCollection`](../schemas/workOrderClose.md#workorderclose-routingitemcollection) | sublist/collection |
| [`workOrderClose-routingItemElement`](../schemas/workOrderClose.md#workorderclose-routingitemelement) | sublist/element |
| [`workOrderCloseCollection`](../schemas/workOrderClose.md#workorderclosecollection) | collection page |
| [`workOrderCloseSelectOptions`](../schemas/workOrderClose.md#workordercloseselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `component` | [`workOrderClose-componentCollection`](../schemas/workOrderClose.md#workorderclose-componentcollection) | [`workOrderClose-componentElement`](../schemas/workOrderClose.md#workorderclose-componentelement) |
| `routingItem` | [`workOrderClose-routingItemCollection`](../schemas/workOrderClose.md#workorderclose-routingitemcollection) | [`workOrderClose-routingItemElement`](../schemas/workOrderClose.md#workorderclose-routingitemelement) |
