# purchaseRequisition

Browser tag `purchaseRequisition` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/purchaseRequisition`, instance `/purchaseRequisition/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/purchaseRequisition` | `operation--purchaseRequisition-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/purchaseRequisition` | `operation--purchaseRequisition-get` | Get list of records. |  | 200 OK → `purchaseRequisitionCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/purchaseRequisition` | `operation--purchaseRequisition-patch` | Update records. | `purchaseRequisitionCollection` | 202 Accepted; default → `nsError` |
| POST | `/purchaseRequisition` | `operation--purchaseRequisition-post` | Insert record. | `purchaseRequisition` | 200 OK → `purchaseRequisition`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/purchaseRequisition` | `operation--purchaseRequisition-put` | Insert or update records. | `purchaseRequisitionCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/purchaseRequisition/{id}` | `operation--purchaseRequisition--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/purchaseRequisition/{id}` | `operation--purchaseRequisition--id--get` | Get record. |  | 200 OK → `purchaseRequisition`; 202 Accepted; default → `nsError` |
| PATCH | `/purchaseRequisition/{id}` | `operation--purchaseRequisition--id--patch` | Update record. | `purchaseRequisition` | 200 OK → `purchaseRequisition`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/purchaseRequisition/{id}` | `operation--purchaseRequisition--id--put` | Insert or update record. | `purchaseRequisition` | 202 Accepted; 204 No Content; default → `nsError` |
| POST | `/purchaseRequisition/{id}/!transform/purchaseOrder` | `operation--purchaseRequisition--id---transform-purchaseOrder-post` | Transform to purchaseOrder. | `purchaseOrder` | 200 OK → `purchaseRequisition`; 202 Accepted; 204 No Content → `purchaseOrder`; default → `nsError` |
| POST | `/purchaseRequisition/{targetId}/!attach/contact/{attachmentId}` | `operation--purchaseRequisition--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` | 202 Accepted; 204 No Content |
| POST | `/purchaseRequisition/{targetId}/!detach/contact/{attachmentId}` | `operation--purchaseRequisition--targetId---detach-contact--attachmentId--post` | Detach a contact. |  | 202 Accepted; 204 No Content |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--purchaseRequisition-delete` | DELETE `/purchaseRequisition` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--purchaseRequisition-get` | GET `/purchaseRequisition` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--purchaseRequisition-patch` | PATCH `/purchaseRequisition` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--purchaseRequisition-post` | POST `/purchaseRequisition` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--purchaseRequisition-put` | PUT `/purchaseRequisition` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--purchaseRequisition--id--delete` | DELETE `/purchaseRequisition/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--purchaseRequisition--id--get` | GET `/purchaseRequisition/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--purchaseRequisition--id--patch` | PATCH `/purchaseRequisition/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--purchaseRequisition--id--put` | PUT `/purchaseRequisition/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--purchaseRequisition--id---transform-purchaseOrder-post` | POST `/purchaseRequisition/{id}/!transform/purchaseOrder` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--purchaseRequisition--targetId---attach-contact--attachmentId--post` | POST `/purchaseRequisition/{targetId}/!attach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--purchaseRequisition--targetId---detach-contact--attachmentId--post` | POST `/purchaseRequisition/{targetId}/!detach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |

## Inline request bodies

### `operation--purchaseRequisition--targetId---attach-contact--attachmentId--post`

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `role` |  | object |  |  |  |  |
| `role.externalId` |  | string |  |  |  |  |
| `role.id` |  | integer | int32 |  |  |  |


## Schema refs

Definitions owned by this record (property tables): [purchaseRequisition schemas](../schemas/purchaseRequisition.md).

| Definition | Role |
| --- | --- |
| [`purchaseRequisition`](../schemas/purchaseRequisition.md#purchaserequisition) | record body |
| [`purchaseRequisition-accountingBookDetailCollection`](../schemas/purchaseRequisition.md#purchaserequisition-accountingbookdetailcollection) | sublist/collection |
| [`purchaseRequisition-accountingBookDetailElement`](../schemas/purchaseRequisition.md#purchaserequisition-accountingbookdetailelement) | sublist/element |
| [`purchaseRequisition-expenseCollection`](../schemas/purchaseRequisition.md#purchaserequisition-expensecollection) | sublist/collection |
| [`purchaseRequisition-expenseElement`](../schemas/purchaseRequisition.md#purchaserequisition-expenseelement) | sublist/element |
| [`purchaseRequisition-item-inventoryDetail`](../schemas/purchaseRequisition.md#purchaserequisition-item-inventorydetail) | related |
| [`purchaseRequisition-item-inventoryDetail-inventoryAssignmentCollection`](../schemas/purchaseRequisition.md#purchaserequisition-item-inventorydetail-inventoryassignmentcollection) | sublist/collection |
| [`purchaseRequisition-item-inventoryDetail-inventoryAssignmentElement`](../schemas/purchaseRequisition.md#purchaserequisition-item-inventorydetail-inventoryassignmentelement) | sublist/element |
| [`purchaseRequisition-itemCollection`](../schemas/purchaseRequisition.md#purchaserequisition-itemcollection) | sublist/collection |
| [`purchaseRequisition-itemElement`](../schemas/purchaseRequisition.md#purchaserequisition-itemelement) | sublist/element |
| [`purchaseRequisitionCollection`](../schemas/purchaseRequisition.md#purchaserequisitioncollection) | collection page |
| [`purchaseRequisitionSelectOptions`](../schemas/purchaseRequisition.md#purchaserequisitionselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)
- [`purchaseOrder`](../schemas/purchaseOrder.md#purchaseorder)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`purchaseRequisition-accountingBookDetailCollection`](../schemas/purchaseRequisition.md#purchaserequisition-accountingbookdetailcollection) | [`purchaseRequisition-accountingBookDetailElement`](../schemas/purchaseRequisition.md#purchaserequisition-accountingbookdetailelement) |
| `expense` | [`purchaseRequisition-expenseCollection`](../schemas/purchaseRequisition.md#purchaserequisition-expensecollection) | [`purchaseRequisition-expenseElement`](../schemas/purchaseRequisition.md#purchaserequisition-expenseelement) |
| `item` | [`purchaseRequisition-itemCollection`](../schemas/purchaseRequisition.md#purchaserequisition-itemcollection) | [`purchaseRequisition-itemElement`](../schemas/purchaseRequisition.md#purchaserequisition-itemelement) |

## Transforms

| Method | Path | Operation ID | Summary | Target | Request body |
| --- | --- | --- | --- | --- | --- |
| POST | `/purchaseRequisition/{id}/!transform/purchaseOrder` | `operation--purchaseRequisition--id---transform-purchaseOrder-post` | Transform to purchaseOrder. | `purchaseOrder` | `purchaseOrder` |

## Attach / detach

| Method | Path | Operation ID | Summary | Request body |
| --- | --- | --- | --- | --- |
| POST | `/purchaseRequisition/{targetId}/!attach/contact/{attachmentId}` | `operation--purchaseRequisition--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` |
| POST | `/purchaseRequisition/{targetId}/!detach/contact/{attachmentId}` | `operation--purchaseRequisition--targetId---detach-contact--attachmentId--post` | Detach a contact. |  |
