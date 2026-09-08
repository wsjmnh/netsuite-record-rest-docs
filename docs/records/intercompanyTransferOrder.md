# intercompanyTransferOrder

Browser tag `intercompanyTransferOrder` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/intercompanyTransferOrder`, instance `/intercompanyTransferOrder/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/intercompanyTransferOrder` | `operation--intercompanyTransferOrder-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/intercompanyTransferOrder` | `operation--intercompanyTransferOrder-get` | Get list of records. |  | 200 OK → `intercompanyTransferOrderCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/intercompanyTransferOrder` | `operation--intercompanyTransferOrder-patch` | Update records. | `intercompanyTransferOrderCollection` | 202 Accepted; default → `nsError` |
| POST | `/intercompanyTransferOrder` | `operation--intercompanyTransferOrder-post` | Insert record. | `intercompanyTransferOrder` | 200 OK → `intercompanyTransferOrder`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/intercompanyTransferOrder` | `operation--intercompanyTransferOrder-put` | Insert or update records. | `intercompanyTransferOrderCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/intercompanyTransferOrder/{id}` | `operation--intercompanyTransferOrder--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/intercompanyTransferOrder/{id}` | `operation--intercompanyTransferOrder--id--get` | Get record. |  | 200 OK → `intercompanyTransferOrder`; 202 Accepted; default → `nsError` |
| PATCH | `/intercompanyTransferOrder/{id}` | `operation--intercompanyTransferOrder--id--patch` | Update record. | `intercompanyTransferOrder` | 200 OK → `intercompanyTransferOrder`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/intercompanyTransferOrder/{id}` | `operation--intercompanyTransferOrder--id--put` | Insert or update record. | `intercompanyTransferOrder` | 202 Accepted; 204 No Content; default → `nsError` |
| POST | `/intercompanyTransferOrder/{id}/!transform/itemFulfillment` | `operation--intercompanyTransferOrder--id---transform-itemFulfillment-post` | Transform to itemFulfillment. | `itemFulfillment` | 200 OK → `intercompanyTransferOrder`; 202 Accepted; 204 No Content → `itemFulfillment`; default → `nsError` |
| POST | `/intercompanyTransferOrder/{id}/!transform/itemReceipt` | `operation--intercompanyTransferOrder--id---transform-itemReceipt-post` | Transform to itemReceipt. | `itemReceipt` | 200 OK → `intercompanyTransferOrder`; 202 Accepted; 204 No Content → `itemReceipt`; default → `nsError` |
| POST | `/intercompanyTransferOrder/{targetId}/!attach/contact/{attachmentId}` | `operation--intercompanyTransferOrder--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` | 202 Accepted; 204 No Content |
| POST | `/intercompanyTransferOrder/{targetId}/!detach/contact/{attachmentId}` | `operation--intercompanyTransferOrder--targetId---detach-contact--attachmentId--post` | Detach a contact. |  | 202 Accepted; 204 No Content |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--intercompanyTransferOrder-delete` | DELETE `/intercompanyTransferOrder` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--intercompanyTransferOrder-get` | GET `/intercompanyTransferOrder` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--intercompanyTransferOrder-patch` | PATCH `/intercompanyTransferOrder` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--intercompanyTransferOrder-post` | POST `/intercompanyTransferOrder` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--intercompanyTransferOrder-put` | PUT `/intercompanyTransferOrder` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--intercompanyTransferOrder--id--delete` | DELETE `/intercompanyTransferOrder/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--intercompanyTransferOrder--id--get` | GET `/intercompanyTransferOrder/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--intercompanyTransferOrder--id--patch` | PATCH `/intercompanyTransferOrder/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--intercompanyTransferOrder--id--put` | PUT `/intercompanyTransferOrder/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--intercompanyTransferOrder--id---transform-itemFulfillment-post` | POST `/intercompanyTransferOrder/{id}/!transform/itemFulfillment` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--intercompanyTransferOrder--id---transform-itemReceipt-post` | POST `/intercompanyTransferOrder/{id}/!transform/itemReceipt` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--intercompanyTransferOrder--targetId---attach-contact--attachmentId--post` | POST `/intercompanyTransferOrder/{targetId}/!attach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--intercompanyTransferOrder--targetId---detach-contact--attachmentId--post` | POST `/intercompanyTransferOrder/{targetId}/!detach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |

## Inline request bodies

### `operation--intercompanyTransferOrder--targetId---attach-contact--attachmentId--post`

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `role` |  | object |  |  |  |  |
| `role.externalId` |  | string |  |  |  |  |
| `role.id` |  | integer | int32 |  |  |  |


## Schema refs

Definitions owned by this record (property tables): [intercompanyTransferOrder schemas](../schemas/intercompanyTransferOrder.md).

| Definition | Role |
| --- | --- |
| [`intercompanyTransferOrder`](../schemas/intercompanyTransferOrder.md#intercompanytransferorder) | record body |
| [`intercompanyTransferOrder-accountingBookDetailCollection`](../schemas/intercompanyTransferOrder.md#intercompanytransferorder-accountingbookdetailcollection) | sublist/collection |
| [`intercompanyTransferOrder-accountingBookDetailElement`](../schemas/intercompanyTransferOrder.md#intercompanytransferorder-accountingbookdetailelement) | sublist/element |
| [`intercompanyTransferOrder-item-inventoryDetail`](../schemas/intercompanyTransferOrder.md#intercompanytransferorder-item-inventorydetail) | related |
| [`intercompanyTransferOrder-item-inventoryDetail-inventoryAssignmentCollection`](../schemas/intercompanyTransferOrder.md#intercompanytransferorder-item-inventorydetail-inventoryassignmentcollection) | sublist/collection |
| [`intercompanyTransferOrder-item-inventoryDetail-inventoryAssignmentElement`](../schemas/intercompanyTransferOrder.md#intercompanytransferorder-item-inventorydetail-inventoryassignmentelement) | sublist/element |
| [`intercompanyTransferOrder-itemCollection`](../schemas/intercompanyTransferOrder.md#intercompanytransferorder-itemcollection) | sublist/collection |
| [`intercompanyTransferOrder-itemElement`](../schemas/intercompanyTransferOrder.md#intercompanytransferorder-itemelement) | sublist/element |
| [`intercompanyTransferOrder-shippingAddress`](../schemas/intercompanyTransferOrder.md#intercompanytransferorder-shippingaddress) | related |
| [`intercompanyTransferOrderCollection`](../schemas/intercompanyTransferOrder.md#intercompanytransferordercollection) | collection page |
| [`intercompanyTransferOrderSelectOptions`](../schemas/intercompanyTransferOrder.md#intercompanytransferorderselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`itemFulfillment`](../schemas/itemFulfillment.md#itemfulfillment)
- [`itemReceipt`](../schemas/itemReceipt.md#itemreceipt)
- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`intercompanyTransferOrder-accountingBookDetailCollection`](../schemas/intercompanyTransferOrder.md#intercompanytransferorder-accountingbookdetailcollection) | [`intercompanyTransferOrder-accountingBookDetailElement`](../schemas/intercompanyTransferOrder.md#intercompanytransferorder-accountingbookdetailelement) |
| `item` | [`intercompanyTransferOrder-itemCollection`](../schemas/intercompanyTransferOrder.md#intercompanytransferorder-itemcollection) | [`intercompanyTransferOrder-itemElement`](../schemas/intercompanyTransferOrder.md#intercompanytransferorder-itemelement) |

## Transforms

| Method | Path | Operation ID | Summary | Target | Request body |
| --- | --- | --- | --- | --- | --- |
| POST | `/intercompanyTransferOrder/{id}/!transform/itemFulfillment` | `operation--intercompanyTransferOrder--id---transform-itemFulfillment-post` | Transform to itemFulfillment. | `itemFulfillment` | `itemFulfillment` |
| POST | `/intercompanyTransferOrder/{id}/!transform/itemReceipt` | `operation--intercompanyTransferOrder--id---transform-itemReceipt-post` | Transform to itemReceipt. | `itemReceipt` | `itemReceipt` |

## Attach / detach

| Method | Path | Operation ID | Summary | Request body |
| --- | --- | --- | --- | --- |
| POST | `/intercompanyTransferOrder/{targetId}/!attach/contact/{attachmentId}` | `operation--intercompanyTransferOrder--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` |
| POST | `/intercompanyTransferOrder/{targetId}/!detach/contact/{attachmentId}` | `operation--intercompanyTransferOrder--targetId---detach-contact--attachmentId--post` | Detach a contact. |  |
