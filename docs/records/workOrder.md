# workOrder

Browser tag `workOrder` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/workOrder`, instance `/workOrder/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/workOrder` | `operation--workOrder-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/workOrder` | `operation--workOrder-get` | Get list of records. |  | 200 OK → `workOrderCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/workOrder` | `operation--workOrder-patch` | Update records. | `workOrderCollection` | 202 Accepted; default → `nsError` |
| POST | `/workOrder` | `operation--workOrder-post` | Insert record. | `workOrder` | 200 OK → `workOrder`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/workOrder` | `operation--workOrder-put` | Insert or update records. | `workOrderCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/workOrder/{id}` | `operation--workOrder--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/workOrder/{id}` | `operation--workOrder--id--get` | Get record. |  | 200 OK → `workOrder`; 202 Accepted; default → `nsError` |
| PATCH | `/workOrder/{id}` | `operation--workOrder--id--patch` | Update record. | `workOrder` | 200 OK → `workOrder`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/workOrder/{id}` | `operation--workOrder--id--put` | Insert or update record. | `workOrder` | 202 Accepted; 204 No Content; default → `nsError` |
| POST | `/workOrder/{id}/!transform/assemblyBuild` | `operation--workOrder--id---transform-assemblyBuild-post` | Transform to assemblyBuild. | `assemblyBuild` | 200 OK → `workOrder`; 202 Accepted; 204 No Content → `assemblyBuild`; default → `nsError` |
| POST | `/workOrder/{id}/!transform/workOrderClose` | `operation--workOrder--id---transform-workOrderClose-post` | Transform to workOrderClose. | `workOrderClose` | 200 OK → `workOrder`; 202 Accepted; 204 No Content → `workOrderClose`; default → `nsError` |
| POST | `/workOrder/{id}/!transform/workOrderCompletion` | `operation--workOrder--id---transform-workOrderCompletion-post` | Transform to workOrderCompletion. | `workOrderCompletion` | 200 OK → `workOrder`; 202 Accepted; 204 No Content → `workOrderCompletion`; default → `nsError` |
| POST | `/workOrder/{id}/!transform/workOrderIssue` | `operation--workOrder--id---transform-workOrderIssue-post` | Transform to workOrderIssue. | `workOrderIssue` | 200 OK → `workOrder`; 202 Accepted; 204 No Content → `workOrderIssue`; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--workOrder-delete` | DELETE `/workOrder` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--workOrder-get` | GET `/workOrder` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--workOrder-patch` | PATCH `/workOrder` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--workOrder-post` | POST `/workOrder` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--workOrder-put` | PUT `/workOrder` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--workOrder--id--delete` | DELETE `/workOrder/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--workOrder--id--get` | GET `/workOrder/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--workOrder--id--patch` | PATCH `/workOrder/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--workOrder--id--put` | PUT `/workOrder/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--workOrder--id---transform-assemblyBuild-post` | POST `/workOrder/{id}/!transform/assemblyBuild` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--workOrder--id---transform-workOrderClose-post` | POST `/workOrder/{id}/!transform/workOrderClose` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--workOrder--id---transform-workOrderCompletion-post` | POST `/workOrder/{id}/!transform/workOrderCompletion` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--workOrder--id---transform-workOrderIssue-post` | POST `/workOrder/{id}/!transform/workOrderIssue` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |

## Schema refs

Definitions owned by this record (property tables): [workOrder schemas](../schemas/workOrder.md).

| Definition | Role |
| --- | --- |
| [`workOrder`](../schemas/workOrder.md#workorder) | record body |
| [`workOrder-accountingBookDetailCollection`](../schemas/workOrder.md#workorder-accountingbookdetailcollection) | sublist/collection |
| [`workOrder-accountingBookDetailElement`](../schemas/workOrder.md#workorder-accountingbookdetailelement) | sublist/element |
| [`workOrder-item-inventoryDetail`](../schemas/workOrder.md#workorder-item-inventorydetail) | related |
| [`workOrder-item-inventoryDetail-inventoryAssignmentCollection`](../schemas/workOrder.md#workorder-item-inventorydetail-inventoryassignmentcollection) | sublist/collection |
| [`workOrder-item-inventoryDetail-inventoryAssignmentElement`](../schemas/workOrder.md#workorder-item-inventorydetail-inventoryassignmentelement) | sublist/element |
| [`workOrder-itemCollection`](../schemas/workOrder.md#workorder-itemcollection) | sublist/collection |
| [`workOrder-itemElement`](../schemas/workOrder.md#workorder-itemelement) | sublist/element |
| [`workOrder-partnersCollection`](../schemas/workOrder.md#workorder-partnerscollection) | sublist/collection |
| [`workOrder-partnersElement`](../schemas/workOrder.md#workorder-partnerselement) | sublist/element |
| [`workOrder-salesTeamCollection`](../schemas/workOrder.md#workorder-salesteamcollection) | sublist/collection |
| [`workOrder-salesTeamElement`](../schemas/workOrder.md#workorder-salesteamelement) | sublist/element |
| [`workOrderCollection`](../schemas/workOrder.md#workordercollection) | collection page |
| [`workOrderSelectOptions`](../schemas/workOrder.md#workorderselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`assemblyBuild`](../schemas/assemblyBuild.md#assemblybuild)
- [`nsError`](../schemas/ns.md#nserror)
- [`workOrderClose`](../schemas/workOrderClose.md#workorderclose)
- [`workOrderCompletion`](../schemas/workOrderCompletion.md#workordercompletion)
- [`workOrderIssue`](../schemas/workOrderIssue.md#workorderissue)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`workOrder-accountingBookDetailCollection`](../schemas/workOrder.md#workorder-accountingbookdetailcollection) | [`workOrder-accountingBookDetailElement`](../schemas/workOrder.md#workorder-accountingbookdetailelement) |
| `item` | [`workOrder-itemCollection`](../schemas/workOrder.md#workorder-itemcollection) | [`workOrder-itemElement`](../schemas/workOrder.md#workorder-itemelement) |
| `partners` | [`workOrder-partnersCollection`](../schemas/workOrder.md#workorder-partnerscollection) | [`workOrder-partnersElement`](../schemas/workOrder.md#workorder-partnerselement) |
| `salesTeam` | [`workOrder-salesTeamCollection`](../schemas/workOrder.md#workorder-salesteamcollection) | [`workOrder-salesTeamElement`](../schemas/workOrder.md#workorder-salesteamelement) |

## Transforms

| Method | Path | Operation ID | Summary | Target | Request body |
| --- | --- | --- | --- | --- | --- |
| POST | `/workOrder/{id}/!transform/assemblyBuild` | `operation--workOrder--id---transform-assemblyBuild-post` | Transform to assemblyBuild. | `assemblyBuild` | `assemblyBuild` |
| POST | `/workOrder/{id}/!transform/workOrderClose` | `operation--workOrder--id---transform-workOrderClose-post` | Transform to workOrderClose. | `workOrderClose` | `workOrderClose` |
| POST | `/workOrder/{id}/!transform/workOrderCompletion` | `operation--workOrder--id---transform-workOrderCompletion-post` | Transform to workOrderCompletion. | `workOrderCompletion` | `workOrderCompletion` |
| POST | `/workOrder/{id}/!transform/workOrderIssue` | `operation--workOrder--id---transform-workOrderIssue-post` | Transform to workOrderIssue. | `workOrderIssue` | `workOrderIssue` |
