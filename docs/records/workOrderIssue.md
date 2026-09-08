# workOrderIssue

Browser tag `workOrderIssue` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/workOrderIssue`, instance `/workOrderIssue/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/workOrderIssue` | `operation--workOrderIssue-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/workOrderIssue` | `operation--workOrderIssue-get` | Get list of records. |  | 200 OK → `workOrderIssueCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/workOrderIssue` | `operation--workOrderIssue-patch` | Update records. | `workOrderIssueCollection` | 202 Accepted; default → `nsError` |
| POST | `/workOrderIssue` | `operation--workOrderIssue-post` | Insert record. | `workOrderIssue` | 200 OK → `workOrderIssue`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/workOrderIssue` | `operation--workOrderIssue-put` | Insert or update records. | `workOrderIssueCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/workOrderIssue/{id}` | `operation--workOrderIssue--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/workOrderIssue/{id}` | `operation--workOrderIssue--id--get` | Get record. |  | 200 OK → `workOrderIssue`; 202 Accepted; default → `nsError` |
| PATCH | `/workOrderIssue/{id}` | `operation--workOrderIssue--id--patch` | Update record. | `workOrderIssue` | 200 OK → `workOrderIssue`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/workOrderIssue/{id}` | `operation--workOrderIssue--id--put` | Insert or update record. | `workOrderIssue` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--workOrderIssue-delete` | DELETE `/workOrderIssue` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--workOrderIssue-get` | GET `/workOrderIssue` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--workOrderIssue-patch` | PATCH `/workOrderIssue` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--workOrderIssue-post` | POST `/workOrderIssue` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--workOrderIssue-put` | PUT `/workOrderIssue` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--workOrderIssue--id--delete` | DELETE `/workOrderIssue/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--workOrderIssue--id--get` | GET `/workOrderIssue/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--workOrderIssue--id--patch` | PATCH `/workOrderIssue/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--workOrderIssue--id--put` | PUT `/workOrderIssue/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [workOrderIssue schemas](../schemas/workOrderIssue.md).

| Definition | Role |
| --- | --- |
| [`workOrderIssue`](../schemas/workOrderIssue.md#workorderissue) | record body |
| [`workOrderIssue-component-componentInventoryDetail`](../schemas/workOrderIssue.md#workorderissue-component-componentinventorydetail) | related |
| [`workOrderIssue-component-componentInventoryDetail-inventoryAssignmentCollection`](../schemas/workOrderIssue.md#workorderissue-component-componentinventorydetail-inventoryassignmentcollection) | sublist/collection |
| [`workOrderIssue-component-componentInventoryDetail-inventoryAssignmentElement`](../schemas/workOrderIssue.md#workorderissue-component-componentinventorydetail-inventoryassignmentelement) | sublist/element |
| [`workOrderIssue-componentCollection`](../schemas/workOrderIssue.md#workorderissue-componentcollection) | sublist/collection |
| [`workOrderIssue-componentElement`](../schemas/workOrderIssue.md#workorderissue-componentelement) | sublist/element |
| [`workOrderIssueCollection`](../schemas/workOrderIssue.md#workorderissuecollection) | collection page |
| [`workOrderIssueSelectOptions`](../schemas/workOrderIssue.md#workorderissueselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `component` | [`workOrderIssue-componentCollection`](../schemas/workOrderIssue.md#workorderissue-componentcollection) | [`workOrderIssue-componentElement`](../schemas/workOrderIssue.md#workorderissue-componentelement) |
