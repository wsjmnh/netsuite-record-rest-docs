# transferOrder

Browser tag `transferOrder` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/transferOrder`, instance `/transferOrder/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/transferOrder` | `operation--transferOrder-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/transferOrder` | `operation--transferOrder-get` | Get list of records. |  | 200 OK → `transferOrderCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/transferOrder` | `operation--transferOrder-patch` | Update records. | `transferOrderCollection` | 202 Accepted; default → `nsError` |
| POST | `/transferOrder` | `operation--transferOrder-post` | Insert record. | `transferOrder` | 200 OK → `transferOrder`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/transferOrder` | `operation--transferOrder-put` | Insert or update records. | `transferOrderCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/transferOrder/{id}` | `operation--transferOrder--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/transferOrder/{id}` | `operation--transferOrder--id--get` | Get record. |  | 200 OK → `transferOrder`; 202 Accepted; default → `nsError` |
| PATCH | `/transferOrder/{id}` | `operation--transferOrder--id--patch` | Update record. | `transferOrder` | 200 OK → `transferOrder`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/transferOrder/{id}` | `operation--transferOrder--id--put` | Insert or update record. | `transferOrder` | 202 Accepted; 204 No Content; default → `nsError` |
| POST | `/transferOrder/{id}/!transform/itemFulfillment` | `operation--transferOrder--id---transform-itemFulfillment-post` | Transform to itemFulfillment. | `itemFulfillment` | 200 OK → `transferOrder`; 202 Accepted; 204 No Content → `itemFulfillment`; default → `nsError` |
| POST | `/transferOrder/{id}/!transform/itemReceipt` | `operation--transferOrder--id---transform-itemReceipt-post` | Transform to itemReceipt. | `itemReceipt` | 200 OK → `transferOrder`; 202 Accepted; 204 No Content → `itemReceipt`; default → `nsError` |
| POST | `/transferOrder/{targetId}/!attach/contact/{attachmentId}` | `operation--transferOrder--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` | 202 Accepted; 204 No Content |
| POST | `/transferOrder/{targetId}/!detach/contact/{attachmentId}` | `operation--transferOrder--targetId---detach-contact--attachmentId--post` | Detach a contact. |  | 202 Accepted; 204 No Content |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--transferOrder-delete` | DELETE `/transferOrder` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--transferOrder-get` | GET `/transferOrder` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--transferOrder-patch` | PATCH `/transferOrder` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--transferOrder-post` | POST `/transferOrder` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--transferOrder-put` | PUT `/transferOrder` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--transferOrder--id--delete` | DELETE `/transferOrder/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--transferOrder--id--get` | GET `/transferOrder/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--transferOrder--id--patch` | PATCH `/transferOrder/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--transferOrder--id--put` | PUT `/transferOrder/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--transferOrder--id---transform-itemFulfillment-post` | POST `/transferOrder/{id}/!transform/itemFulfillment` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--transferOrder--id---transform-itemReceipt-post` | POST `/transferOrder/{id}/!transform/itemReceipt` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--transferOrder--targetId---attach-contact--attachmentId--post` | POST `/transferOrder/{targetId}/!attach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--transferOrder--targetId---detach-contact--attachmentId--post` | POST `/transferOrder/{targetId}/!detach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |

## Inline request bodies

### `operation--transferOrder--targetId---attach-contact--attachmentId--post`

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `role` |  | object |  |  |  |  |
| `role.externalId` |  | string |  |  |  |  |
| `role.id` |  | integer | int32 |  |  |  |


## Schema refs

Definitions owned by this record (property tables): [transferOrder schemas](../schemas/transferOrder.md).

| Definition | Role |
| --- | --- |
| [`transferOrder`](../schemas/transferOrder.md#transferorder) | record body |
| [`transferOrder-accountingBookDetailCollection`](../schemas/transferOrder.md#transferorder-accountingbookdetailcollection) | sublist/collection |
| [`transferOrder-accountingBookDetailElement`](../schemas/transferOrder.md#transferorder-accountingbookdetailelement) | sublist/element |
| [`transferOrder-item-inventoryDetail`](../schemas/transferOrder.md#transferorder-item-inventorydetail) | related |
| [`transferOrder-item-inventoryDetail-inventoryAssignmentCollection`](../schemas/transferOrder.md#transferorder-item-inventorydetail-inventoryassignmentcollection) | sublist/collection |
| [`transferOrder-item-inventoryDetail-inventoryAssignmentElement`](../schemas/transferOrder.md#transferorder-item-inventorydetail-inventoryassignmentelement) | sublist/element |
| [`transferOrder-itemCollection`](../schemas/transferOrder.md#transferorder-itemcollection) | sublist/collection |
| [`transferOrder-itemElement`](../schemas/transferOrder.md#transferorder-itemelement) | sublist/element |
| [`transferOrder-shippingAddress`](../schemas/transferOrder.md#transferorder-shippingaddress) | related |
| [`transferOrderCollection`](../schemas/transferOrder.md#transferordercollection) | collection page |
| [`transferOrderSelectOptions`](../schemas/transferOrder.md#transferorderselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`itemFulfillment`](../schemas/itemFulfillment.md#itemfulfillment)
- [`itemReceipt`](../schemas/itemReceipt.md#itemreceipt)
- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`transferOrder-accountingBookDetailCollection`](../schemas/transferOrder.md#transferorder-accountingbookdetailcollection) | [`transferOrder-accountingBookDetailElement`](../schemas/transferOrder.md#transferorder-accountingbookdetailelement) |
| `item` | [`transferOrder-itemCollection`](../schemas/transferOrder.md#transferorder-itemcollection) | [`transferOrder-itemElement`](../schemas/transferOrder.md#transferorder-itemelement) |

## Transforms

| Method | Path | Operation ID | Summary | Target | Request body |
| --- | --- | --- | --- | --- | --- |
| POST | `/transferOrder/{id}/!transform/itemFulfillment` | `operation--transferOrder--id---transform-itemFulfillment-post` | Transform to itemFulfillment. | `itemFulfillment` | `itemFulfillment` |
| POST | `/transferOrder/{id}/!transform/itemReceipt` | `operation--transferOrder--id---transform-itemReceipt-post` | Transform to itemReceipt. | `itemReceipt` | `itemReceipt` |

## Attach / detach

| Method | Path | Operation ID | Summary | Request body |
| --- | --- | --- | --- | --- |
| POST | `/transferOrder/{targetId}/!attach/contact/{attachmentId}` | `operation--transferOrder--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` |
| POST | `/transferOrder/{targetId}/!detach/contact/{attachmentId}` | `operation--transferOrder--targetId---detach-contact--attachmentId--post` | Detach a contact. |  |
