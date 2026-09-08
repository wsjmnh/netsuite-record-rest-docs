# workOrderCompletion

Browser tag `workOrderCompletion` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/workOrderCompletion`, instance `/workOrderCompletion/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/workOrderCompletion` | `operation--workOrderCompletion-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/workOrderCompletion` | `operation--workOrderCompletion-get` | Get list of records. |  | 200 OK → `workOrderCompletionCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/workOrderCompletion` | `operation--workOrderCompletion-patch` | Update records. | `workOrderCompletionCollection` | 202 Accepted; default → `nsError` |
| POST | `/workOrderCompletion` | `operation--workOrderCompletion-post` | Insert record. | `workOrderCompletion` | 200 OK → `workOrderCompletion`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/workOrderCompletion` | `operation--workOrderCompletion-put` | Insert or update records. | `workOrderCompletionCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/workOrderCompletion/{id}` | `operation--workOrderCompletion--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/workOrderCompletion/{id}` | `operation--workOrderCompletion--id--get` | Get record. |  | 200 OK → `workOrderCompletion`; 202 Accepted; default → `nsError` |
| PATCH | `/workOrderCompletion/{id}` | `operation--workOrderCompletion--id--patch` | Update record. | `workOrderCompletion` | 200 OK → `workOrderCompletion`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/workOrderCompletion/{id}` | `operation--workOrderCompletion--id--put` | Insert or update record. | `workOrderCompletion` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--workOrderCompletion-delete` | DELETE `/workOrderCompletion` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--workOrderCompletion-get` | GET `/workOrderCompletion` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--workOrderCompletion-patch` | PATCH `/workOrderCompletion` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--workOrderCompletion-post` | POST `/workOrderCompletion` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--workOrderCompletion-put` | PUT `/workOrderCompletion` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--workOrderCompletion--id--delete` | DELETE `/workOrderCompletion/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--workOrderCompletion--id--get` | GET `/workOrderCompletion/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--workOrderCompletion--id--patch` | PATCH `/workOrderCompletion/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--workOrderCompletion--id--put` | PUT `/workOrderCompletion/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [workOrderCompletion schemas](../schemas/workOrderCompletion.md).

| Definition | Role |
| --- | --- |
| [`workOrderCompletion`](../schemas/workOrderCompletion.md#workordercompletion) | record body |
| [`workOrderCompletion-accountingBookDetailCollection`](../schemas/workOrderCompletion.md#workordercompletion-accountingbookdetailcollection) | sublist/collection |
| [`workOrderCompletion-accountingBookDetailElement`](../schemas/workOrderCompletion.md#workordercompletion-accountingbookdetailelement) | sublist/element |
| [`workOrderCompletion-component-componentInventoryDetail`](../schemas/workOrderCompletion.md#workordercompletion-component-componentinventorydetail) | related |
| [`workOrderCompletion-component-componentInventoryDetail-inventoryAssignmentCollection`](../schemas/workOrderCompletion.md#workordercompletion-component-componentinventorydetail-inventoryassignmentcollection) | sublist/collection |
| [`workOrderCompletion-component-componentInventoryDetail-inventoryAssignmentElement`](../schemas/workOrderCompletion.md#workordercompletion-component-componentinventorydetail-inventoryassignmentelement) | sublist/element |
| [`workOrderCompletion-componentCollection`](../schemas/workOrderCompletion.md#workordercompletion-componentcollection) | sublist/collection |
| [`workOrderCompletion-componentElement`](../schemas/workOrderCompletion.md#workordercompletion-componentelement) | sublist/element |
| [`workOrderCompletion-inventoryDetail`](../schemas/workOrderCompletion.md#workordercompletion-inventorydetail) | related |
| [`workOrderCompletion-inventoryDetail-inventoryAssignmentCollection`](../schemas/workOrderCompletion.md#workordercompletion-inventorydetail-inventoryassignmentcollection) | sublist/collection |
| [`workOrderCompletion-inventoryDetail-inventoryAssignmentElement`](../schemas/workOrderCompletion.md#workordercompletion-inventorydetail-inventoryassignmentelement) | sublist/element |
| [`workOrderCompletion-operationCollection`](../schemas/workOrderCompletion.md#workordercompletion-operationcollection) | sublist/collection |
| [`workOrderCompletion-operationElement`](../schemas/workOrderCompletion.md#workordercompletion-operationelement) | sublist/element |
| [`workOrderCompletionCollection`](../schemas/workOrderCompletion.md#workordercompletioncollection) | collection page |
| [`workOrderCompletionSelectOptions`](../schemas/workOrderCompletion.md#workordercompletionselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`workOrderCompletion-accountingBookDetailCollection`](../schemas/workOrderCompletion.md#workordercompletion-accountingbookdetailcollection) | [`workOrderCompletion-accountingBookDetailElement`](../schemas/workOrderCompletion.md#workordercompletion-accountingbookdetailelement) |
| `component` | [`workOrderCompletion-componentCollection`](../schemas/workOrderCompletion.md#workordercompletion-componentcollection) | [`workOrderCompletion-componentElement`](../schemas/workOrderCompletion.md#workordercompletion-componentelement) |
| `operation` | [`workOrderCompletion-operationCollection`](../schemas/workOrderCompletion.md#workordercompletion-operationcollection) | [`workOrderCompletion-operationElement`](../schemas/workOrderCompletion.md#workordercompletion-operationelement) |
