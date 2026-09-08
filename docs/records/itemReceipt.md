# itemReceipt

Browser tag `itemReceipt` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/itemReceipt`, instance `/itemReceipt/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/itemReceipt` | `operation--itemReceipt-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/itemReceipt` | `operation--itemReceipt-get` | Get list of records. |  | 200 OK → `itemReceiptCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/itemReceipt` | `operation--itemReceipt-patch` | Update records. | `itemReceiptCollection` | 202 Accepted; default → `nsError` |
| POST | `/itemReceipt` | `operation--itemReceipt-post` | Insert record. | `itemReceipt` | 200 OK → `itemReceipt`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/itemReceipt` | `operation--itemReceipt-put` | Insert or update records. | `itemReceiptCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/itemReceipt/{id}` | `operation--itemReceipt--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/itemReceipt/{id}` | `operation--itemReceipt--id--get` | Get record. |  | 200 OK → `itemReceipt`; 202 Accepted; default → `nsError` |
| PATCH | `/itemReceipt/{id}` | `operation--itemReceipt--id--patch` | Update record. | `itemReceipt` | 200 OK → `itemReceipt`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/itemReceipt/{id}` | `operation--itemReceipt--id--put` | Insert or update record. | `itemReceipt` | 202 Accepted; 204 No Content; default → `nsError` |
| POST | `/itemReceipt/{targetId}/!attach/contact/{attachmentId}` | `operation--itemReceipt--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` | 202 Accepted; 204 No Content |
| POST | `/itemReceipt/{targetId}/!detach/contact/{attachmentId}` | `operation--itemReceipt--targetId---detach-contact--attachmentId--post` | Detach a contact. |  | 202 Accepted; 204 No Content |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--itemReceipt-delete` | DELETE `/itemReceipt` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemReceipt-get` | GET `/itemReceipt` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemReceipt-patch` | PATCH `/itemReceipt` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemReceipt-post` | POST `/itemReceipt` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--itemReceipt-put` | PUT `/itemReceipt` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemReceipt--id--delete` | DELETE `/itemReceipt/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemReceipt--id--get` | GET `/itemReceipt/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemReceipt--id--patch` | PATCH `/itemReceipt/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--itemReceipt--id--put` | PUT `/itemReceipt/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--itemReceipt--targetId---attach-contact--attachmentId--post` | POST `/itemReceipt/{targetId}/!attach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemReceipt--targetId---detach-contact--attachmentId--post` | POST `/itemReceipt/{targetId}/!detach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |

## Inline request bodies

### `operation--itemReceipt--targetId---attach-contact--attachmentId--post`

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `role` |  | object |  |  |  |  |
| `role.externalId` |  | string |  |  |  |  |
| `role.id` |  | integer | int32 |  |  |  |


## Schema refs

Definitions owned by this record (property tables): [itemReceipt schemas](../schemas/itemReceipt.md).

| Definition | Role |
| --- | --- |
| [`itemReceipt`](../schemas/itemReceipt.md#itemreceipt) | record body |
| [`itemReceipt-accountingBookDetailCollection`](../schemas/itemReceipt.md#itemreceipt-accountingbookdetailcollection) | sublist/collection |
| [`itemReceipt-accountingBookDetailElement`](../schemas/itemReceipt.md#itemreceipt-accountingbookdetailelement) | sublist/element |
| [`itemReceipt-appliedRulesCollection`](../schemas/itemReceipt.md#itemreceipt-appliedrulescollection) | sublist/collection |
| [`itemReceipt-appliedRulesElement`](../schemas/itemReceipt.md#itemreceipt-appliedruleselement) | sublist/element |
| [`itemReceipt-expenseCollection`](../schemas/itemReceipt.md#itemreceipt-expensecollection) | sublist/collection |
| [`itemReceipt-expenseElement`](../schemas/itemReceipt.md#itemreceipt-expenseelement) | sublist/element |
| [`itemReceipt-item-inventoryDetail`](../schemas/itemReceipt.md#itemreceipt-item-inventorydetail) | related |
| [`itemReceipt-item-inventoryDetail-inventoryAssignmentCollection`](../schemas/itemReceipt.md#itemreceipt-item-inventorydetail-inventoryassignmentcollection) | sublist/collection |
| [`itemReceipt-item-inventoryDetail-inventoryAssignmentElement`](../schemas/itemReceipt.md#itemreceipt-item-inventorydetail-inventoryassignmentelement) | sublist/element |
| [`itemReceipt-item-landedCost`](../schemas/itemReceipt.md#itemreceipt-item-landedcost) | related |
| [`itemReceipt-item-landedCost-landedCostDataCollection`](../schemas/itemReceipt.md#itemreceipt-item-landedcost-landedcostdatacollection) | sublist/collection |
| [`itemReceipt-item-landedCost-landedCostDataElement`](../schemas/itemReceipt.md#itemreceipt-item-landedcost-landedcostdataelement) | sublist/element |
| [`itemReceipt-itemCollection`](../schemas/itemReceipt.md#itemreceipt-itemcollection) | sublist/collection |
| [`itemReceipt-itemElement`](../schemas/itemReceipt.md#itemreceipt-itemelement) | sublist/element |
| [`itemReceipt-landedCostsCollection`](../schemas/itemReceipt.md#itemreceipt-landedcostscollection) | sublist/collection |
| [`itemReceipt-landedCostsElement`](../schemas/itemReceipt.md#itemreceipt-landedcostselement) | sublist/element |
| [`itemReceiptCollection`](../schemas/itemReceipt.md#itemreceiptcollection) | collection page |
| [`itemReceiptSelectOptions`](../schemas/itemReceipt.md#itemreceiptselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`itemReceipt-accountingBookDetailCollection`](../schemas/itemReceipt.md#itemreceipt-accountingbookdetailcollection) | [`itemReceipt-accountingBookDetailElement`](../schemas/itemReceipt.md#itemreceipt-accountingbookdetailelement) |
| `appliedRules` | [`itemReceipt-appliedRulesCollection`](../schemas/itemReceipt.md#itemreceipt-appliedrulescollection) | [`itemReceipt-appliedRulesElement`](../schemas/itemReceipt.md#itemreceipt-appliedruleselement) |
| `expense` | [`itemReceipt-expenseCollection`](../schemas/itemReceipt.md#itemreceipt-expensecollection) | [`itemReceipt-expenseElement`](../schemas/itemReceipt.md#itemreceipt-expenseelement) |
| `item` | [`itemReceipt-itemCollection`](../schemas/itemReceipt.md#itemreceipt-itemcollection) | [`itemReceipt-itemElement`](../schemas/itemReceipt.md#itemreceipt-itemelement) |
| `landedCosts` | [`itemReceipt-landedCostsCollection`](../schemas/itemReceipt.md#itemreceipt-landedcostscollection) | [`itemReceipt-landedCostsElement`](../schemas/itemReceipt.md#itemreceipt-landedcostselement) |

## Attach / detach

| Method | Path | Operation ID | Summary | Request body |
| --- | --- | --- | --- | --- |
| POST | `/itemReceipt/{targetId}/!attach/contact/{attachmentId}` | `operation--itemReceipt--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` |
| POST | `/itemReceipt/{targetId}/!detach/contact/{attachmentId}` | `operation--itemReceipt--targetId---detach-contact--attachmentId--post` | Detach a contact. |  |
