# purchaseOrder

Browser tag `purchaseOrder` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/purchaseOrder`, instance `/purchaseOrder/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/purchaseOrder` | `operation--purchaseOrder-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/purchaseOrder` | `operation--purchaseOrder-get` | Get list of records. |  | 200 OK → `purchaseOrderCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/purchaseOrder` | `operation--purchaseOrder-patch` | Update records. | `purchaseOrderCollection` | 202 Accepted; default → `nsError` |
| POST | `/purchaseOrder` | `operation--purchaseOrder-post` | Insert record. | `purchaseOrder` | 200 OK → `purchaseOrder`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/purchaseOrder` | `operation--purchaseOrder-put` | Insert or update records. | `purchaseOrderCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/purchaseOrder/{id}` | `operation--purchaseOrder--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/purchaseOrder/{id}` | `operation--purchaseOrder--id--get` | Get record. |  | 200 OK → `purchaseOrder`; 202 Accepted; default → `nsError` |
| PATCH | `/purchaseOrder/{id}` | `operation--purchaseOrder--id--patch` | Update record. | `purchaseOrder` | 200 OK → `purchaseOrder`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/purchaseOrder/{id}` | `operation--purchaseOrder--id--put` | Insert or update record. | `purchaseOrder` | 202 Accepted; 204 No Content; default → `nsError` |
| POST | `/purchaseOrder/{id}/!transform/itemReceipt` | `operation--purchaseOrder--id---transform-itemReceipt-post` | Transform to itemReceipt. | `itemReceipt` | 200 OK → `purchaseOrder`; 202 Accepted; 204 No Content → `itemReceipt`; default → `nsError` |
| POST | `/purchaseOrder/{id}/!transform/vendorBill` | `operation--purchaseOrder--id---transform-vendorBill-post` | Transform to vendorBill. | `vendorBill` | 200 OK → `purchaseOrder`; 202 Accepted; 204 No Content → `vendorBill`; default → `nsError` |
| POST | `/purchaseOrder/{id}/!transform/vendorReturnAuthorization` | `operation--purchaseOrder--id---transform-vendorReturnAuthorization-post` | Transform to vendorReturnAuthorization. | `vendorReturnAuthorization` | 200 OK → `purchaseOrder`; 202 Accepted; 204 No Content → `vendorReturnAuthorization`; default → `nsError` |
| POST | `/purchaseOrder/{targetId}/!attach/contact/{attachmentId}` | `operation--purchaseOrder--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` | 202 Accepted; 204 No Content |
| POST | `/purchaseOrder/{targetId}/!detach/contact/{attachmentId}` | `operation--purchaseOrder--targetId---detach-contact--attachmentId--post` | Detach a contact. |  | 202 Accepted; 204 No Content |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--purchaseOrder-delete` | DELETE `/purchaseOrder` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--purchaseOrder-get` | GET `/purchaseOrder` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--purchaseOrder-patch` | PATCH `/purchaseOrder` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--purchaseOrder-post` | POST `/purchaseOrder` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--purchaseOrder-put` | PUT `/purchaseOrder` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--purchaseOrder--id--delete` | DELETE `/purchaseOrder/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--purchaseOrder--id--get` | GET `/purchaseOrder/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--purchaseOrder--id--patch` | PATCH `/purchaseOrder/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--purchaseOrder--id--put` | PUT `/purchaseOrder/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--purchaseOrder--id---transform-itemReceipt-post` | POST `/purchaseOrder/{id}/!transform/itemReceipt` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--purchaseOrder--id---transform-vendorBill-post` | POST `/purchaseOrder/{id}/!transform/vendorBill` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--purchaseOrder--id---transform-vendorReturnAuthorization-post` | POST `/purchaseOrder/{id}/!transform/vendorReturnAuthorization` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--purchaseOrder--targetId---attach-contact--attachmentId--post` | POST `/purchaseOrder/{targetId}/!attach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--purchaseOrder--targetId---detach-contact--attachmentId--post` | POST `/purchaseOrder/{targetId}/!detach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |

## Inline request bodies

### `operation--purchaseOrder--targetId---attach-contact--attachmentId--post`

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `role` |  | object |  |  |  |  |
| `role.externalId` |  | string |  |  |  |  |
| `role.id` |  | integer | int32 |  |  |  |


## Schema refs

Definitions owned by this record (property tables): [purchaseOrder schemas](../schemas/purchaseOrder.md).

| Definition | Role |
| --- | --- |
| [`purchaseOrder`](../schemas/purchaseOrder.md#purchaseorder) | record body |
| [`purchaseOrder-accountingBookDetailCollection`](../schemas/purchaseOrder.md#purchaseorder-accountingbookdetailcollection) | sublist/collection |
| [`purchaseOrder-accountingBookDetailElement`](../schemas/purchaseOrder.md#purchaseorder-accountingbookdetailelement) | sublist/element |
| [`purchaseOrder-appliedRulesCollection`](../schemas/purchaseOrder.md#purchaseorder-appliedrulescollection) | sublist/collection |
| [`purchaseOrder-appliedRulesElement`](../schemas/purchaseOrder.md#purchaseorder-appliedruleselement) | sublist/element |
| [`purchaseOrder-billingAddress`](../schemas/purchaseOrder.md#purchaseorder-billingaddress) | related |
| [`purchaseOrder-expenseCollection`](../schemas/purchaseOrder.md#purchaseorder-expensecollection) | sublist/collection |
| [`purchaseOrder-expenseElement`](../schemas/purchaseOrder.md#purchaseorder-expenseelement) | sublist/element |
| [`purchaseOrder-item-inventoryDetail`](../schemas/purchaseOrder.md#purchaseorder-item-inventorydetail) | related |
| [`purchaseOrder-item-inventoryDetail-inventoryAssignmentCollection`](../schemas/purchaseOrder.md#purchaseorder-item-inventorydetail-inventoryassignmentcollection) | sublist/collection |
| [`purchaseOrder-item-inventoryDetail-inventoryAssignmentElement`](../schemas/purchaseOrder.md#purchaseorder-item-inventorydetail-inventoryassignmentelement) | sublist/element |
| [`purchaseOrder-itemCollection`](../schemas/purchaseOrder.md#purchaseorder-itemcollection) | sublist/collection |
| [`purchaseOrder-itemElement`](../schemas/purchaseOrder.md#purchaseorder-itemelement) | sublist/element |
| [`purchaseOrder-shippingAddress`](../schemas/purchaseOrder.md#purchaseorder-shippingaddress) | related |
| [`purchaseOrder-taxDetailsCollection`](../schemas/purchaseOrder.md#purchaseorder-taxdetailscollection) | sublist/collection |
| [`purchaseOrder-taxDetailsElement`](../schemas/purchaseOrder.md#purchaseorder-taxdetailselement) | sublist/element |
| [`purchaseOrderCollection`](../schemas/purchaseOrder.md#purchaseordercollection) | collection page |
| [`purchaseOrderSelectOptions`](../schemas/purchaseOrder.md#purchaseorderselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`itemReceipt`](../schemas/itemReceipt.md#itemreceipt)
- [`nsError`](../schemas/ns.md#nserror)
- [`vendorBill`](../schemas/vendorBill.md#vendorbill)
- [`vendorReturnAuthorization`](../schemas/vendorReturnAuthorization.md#vendorreturnauthorization)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`purchaseOrder-accountingBookDetailCollection`](../schemas/purchaseOrder.md#purchaseorder-accountingbookdetailcollection) | [`purchaseOrder-accountingBookDetailElement`](../schemas/purchaseOrder.md#purchaseorder-accountingbookdetailelement) |
| `appliedRules` | [`purchaseOrder-appliedRulesCollection`](../schemas/purchaseOrder.md#purchaseorder-appliedrulescollection) | [`purchaseOrder-appliedRulesElement`](../schemas/purchaseOrder.md#purchaseorder-appliedruleselement) |
| `expense` | [`purchaseOrder-expenseCollection`](../schemas/purchaseOrder.md#purchaseorder-expensecollection) | [`purchaseOrder-expenseElement`](../schemas/purchaseOrder.md#purchaseorder-expenseelement) |
| `item` | [`purchaseOrder-itemCollection`](../schemas/purchaseOrder.md#purchaseorder-itemcollection) | [`purchaseOrder-itemElement`](../schemas/purchaseOrder.md#purchaseorder-itemelement) |
| `taxDetails` | [`purchaseOrder-taxDetailsCollection`](../schemas/purchaseOrder.md#purchaseorder-taxdetailscollection) | [`purchaseOrder-taxDetailsElement`](../schemas/purchaseOrder.md#purchaseorder-taxdetailselement) |

## Transforms

| Method | Path | Operation ID | Summary | Target | Request body |
| --- | --- | --- | --- | --- | --- |
| POST | `/purchaseOrder/{id}/!transform/itemReceipt` | `operation--purchaseOrder--id---transform-itemReceipt-post` | Transform to itemReceipt. | `itemReceipt` | `itemReceipt` |
| POST | `/purchaseOrder/{id}/!transform/vendorBill` | `operation--purchaseOrder--id---transform-vendorBill-post` | Transform to vendorBill. | `vendorBill` | `vendorBill` |
| POST | `/purchaseOrder/{id}/!transform/vendorReturnAuthorization` | `operation--purchaseOrder--id---transform-vendorReturnAuthorization-post` | Transform to vendorReturnAuthorization. | `vendorReturnAuthorization` | `vendorReturnAuthorization` |

## Attach / detach

| Method | Path | Operation ID | Summary | Request body |
| --- | --- | --- | --- | --- |
| POST | `/purchaseOrder/{targetId}/!attach/contact/{attachmentId}` | `operation--purchaseOrder--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` |
| POST | `/purchaseOrder/{targetId}/!detach/contact/{attachmentId}` | `operation--purchaseOrder--targetId---detach-contact--attachmentId--post` | Detach a contact. |  |
