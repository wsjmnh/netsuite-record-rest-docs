# estimate

Browser tag `estimate` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/estimate`, instance `/estimate/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/estimate` | `operation--estimate-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/estimate` | `operation--estimate-get` | Get list of records. |  | 200 OK → `estimateCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/estimate` | `operation--estimate-patch` | Update records. | `estimateCollection` | 202 Accepted; default → `nsError` |
| POST | `/estimate` | `operation--estimate-post` | Insert record. | `estimate` | 200 OK → `estimate`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/estimate` | `operation--estimate-put` | Insert or update records. | `estimateCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/estimate/{id}` | `operation--estimate--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/estimate/{id}` | `operation--estimate--id--get` | Get record. |  | 200 OK → `estimate`; 202 Accepted; default → `nsError` |
| PATCH | `/estimate/{id}` | `operation--estimate--id--patch` | Update record. | `estimate` | 200 OK → `estimate`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/estimate/{id}` | `operation--estimate--id--put` | Insert or update record. | `estimate` | 202 Accepted; 204 No Content; default → `nsError` |
| POST | `/estimate/{id}/!transform/cashSale` | `operation--estimate--id---transform-cashSale-post` | Transform to cashSale. | `cashSale` | 200 OK → `estimate`; 202 Accepted; 204 No Content → `cashSale`; default → `nsError` |
| POST | `/estimate/{id}/!transform/invoice` | `operation--estimate--id---transform-invoice-post` | Transform to invoice. | `invoice` | 200 OK → `estimate`; 202 Accepted; 204 No Content → `invoice`; default → `nsError` |
| POST | `/estimate/{id}/!transform/salesOrder` | `operation--estimate--id---transform-salesOrder-post` | Transform to salesOrder. | `salesOrder` | 200 OK → `estimate`; 202 Accepted; 204 No Content → `salesOrder`; default → `nsError` |
| POST | `/estimate/{targetId}/!attach/contact/{attachmentId}` | `operation--estimate--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` | 202 Accepted; 204 No Content |
| POST | `/estimate/{targetId}/!detach/contact/{attachmentId}` | `operation--estimate--targetId---detach-contact--attachmentId--post` | Detach a contact. |  | 202 Accepted; 204 No Content |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--estimate-delete` | DELETE `/estimate` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--estimate-get` | GET `/estimate` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--estimate-patch` | PATCH `/estimate` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--estimate-post` | POST `/estimate` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--estimate-put` | PUT `/estimate` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--estimate--id--delete` | DELETE `/estimate/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--estimate--id--get` | GET `/estimate/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--estimate--id--patch` | PATCH `/estimate/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--estimate--id--put` | PUT `/estimate/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--estimate--id---transform-cashSale-post` | POST `/estimate/{id}/!transform/cashSale` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--estimate--id---transform-invoice-post` | POST `/estimate/{id}/!transform/invoice` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--estimate--id---transform-salesOrder-post` | POST `/estimate/{id}/!transform/salesOrder` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--estimate--targetId---attach-contact--attachmentId--post` | POST `/estimate/{targetId}/!attach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--estimate--targetId---detach-contact--attachmentId--post` | POST `/estimate/{targetId}/!detach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |

## Inline request bodies

### `operation--estimate--targetId---attach-contact--attachmentId--post`

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `role` |  | object |  |  |  |  |
| `role.externalId` |  | string |  |  |  |  |
| `role.id` |  | integer | int32 |  |  |  |


## Schema refs

Definitions owned by this record (property tables): [estimate schemas](../schemas/estimate.md).

| Definition | Role |
| --- | --- |
| [`estimate`](../schemas/estimate.md#estimate) | record body |
| [`estimate-accountingBookDetailCollection`](../schemas/estimate.md#estimate-accountingbookdetailcollection) | sublist/collection |
| [`estimate-accountingBookDetailElement`](../schemas/estimate.md#estimate-accountingbookdetailelement) | sublist/element |
| [`estimate-appliedRulesCollection`](../schemas/estimate.md#estimate-appliedrulescollection) | sublist/collection |
| [`estimate-appliedRulesElement`](../schemas/estimate.md#estimate-appliedruleselement) | sublist/element |
| [`estimate-billingAddress`](../schemas/estimate.md#estimate-billingaddress) | related |
| [`estimate-item-inventoryDetail`](../schemas/estimate.md#estimate-item-inventorydetail) | related |
| [`estimate-item-inventoryDetail-inventoryAssignmentCollection`](../schemas/estimate.md#estimate-item-inventorydetail-inventoryassignmentcollection) | sublist/collection |
| [`estimate-item-inventoryDetail-inventoryAssignmentElement`](../schemas/estimate.md#estimate-item-inventorydetail-inventoryassignmentelement) | sublist/element |
| [`estimate-itemCollection`](../schemas/estimate.md#estimate-itemcollection) | sublist/collection |
| [`estimate-itemElement`](../schemas/estimate.md#estimate-itemelement) | sublist/element |
| [`estimate-partnersCollection`](../schemas/estimate.md#estimate-partnerscollection) | sublist/collection |
| [`estimate-partnersElement`](../schemas/estimate.md#estimate-partnerselement) | sublist/element |
| [`estimate-promotionsCollection`](../schemas/estimate.md#estimate-promotionscollection) | sublist/collection |
| [`estimate-promotionsElement`](../schemas/estimate.md#estimate-promotionselement) | sublist/element |
| [`estimate-salesTeamCollection`](../schemas/estimate.md#estimate-salesteamcollection) | sublist/collection |
| [`estimate-salesTeamElement`](../schemas/estimate.md#estimate-salesteamelement) | sublist/element |
| [`estimate-shipGroupCollection`](../schemas/estimate.md#estimate-shipgroupcollection) | sublist/collection |
| [`estimate-shipGroupElement`](../schemas/estimate.md#estimate-shipgroupelement) | sublist/element |
| [`estimate-shippingAddress`](../schemas/estimate.md#estimate-shippingaddress) | related |
| [`estimate-taxDetailsCollection`](../schemas/estimate.md#estimate-taxdetailscollection) | sublist/collection |
| [`estimate-taxDetailsElement`](../schemas/estimate.md#estimate-taxdetailselement) | sublist/element |
| [`estimateCollection`](../schemas/estimate.md#estimatecollection) | collection page |
| [`estimateSelectOptions`](../schemas/estimate.md#estimateselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`cashSale`](../schemas/cashSale.md#cashsale)
- [`invoice`](../schemas/invoice.md#invoice)
- [`nsError`](../schemas/ns.md#nserror)
- [`salesOrder`](../schemas/salesOrder.md#salesorder)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`estimate-accountingBookDetailCollection`](../schemas/estimate.md#estimate-accountingbookdetailcollection) | [`estimate-accountingBookDetailElement`](../schemas/estimate.md#estimate-accountingbookdetailelement) |
| `appliedRules` | [`estimate-appliedRulesCollection`](../schemas/estimate.md#estimate-appliedrulescollection) | [`estimate-appliedRulesElement`](../schemas/estimate.md#estimate-appliedruleselement) |
| `item` | [`estimate-itemCollection`](../schemas/estimate.md#estimate-itemcollection) | [`estimate-itemElement`](../schemas/estimate.md#estimate-itemelement) |
| `partners` | [`estimate-partnersCollection`](../schemas/estimate.md#estimate-partnerscollection) | [`estimate-partnersElement`](../schemas/estimate.md#estimate-partnerselement) |
| `promotions` | [`estimate-promotionsCollection`](../schemas/estimate.md#estimate-promotionscollection) | [`estimate-promotionsElement`](../schemas/estimate.md#estimate-promotionselement) |
| `salesTeam` | [`estimate-salesTeamCollection`](../schemas/estimate.md#estimate-salesteamcollection) | [`estimate-salesTeamElement`](../schemas/estimate.md#estimate-salesteamelement) |
| `shipGroup` | [`estimate-shipGroupCollection`](../schemas/estimate.md#estimate-shipgroupcollection) | [`estimate-shipGroupElement`](../schemas/estimate.md#estimate-shipgroupelement) |
| `taxDetails` | [`estimate-taxDetailsCollection`](../schemas/estimate.md#estimate-taxdetailscollection) | [`estimate-taxDetailsElement`](../schemas/estimate.md#estimate-taxdetailselement) |

## Transforms

| Method | Path | Operation ID | Summary | Target | Request body |
| --- | --- | --- | --- | --- | --- |
| POST | `/estimate/{id}/!transform/cashSale` | `operation--estimate--id---transform-cashSale-post` | Transform to cashSale. | `cashSale` | `cashSale` |
| POST | `/estimate/{id}/!transform/invoice` | `operation--estimate--id---transform-invoice-post` | Transform to invoice. | `invoice` | `invoice` |
| POST | `/estimate/{id}/!transform/salesOrder` | `operation--estimate--id---transform-salesOrder-post` | Transform to salesOrder. | `salesOrder` | `salesOrder` |

## Attach / detach

| Method | Path | Operation ID | Summary | Request body |
| --- | --- | --- | --- | --- |
| POST | `/estimate/{targetId}/!attach/contact/{attachmentId}` | `operation--estimate--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` |
| POST | `/estimate/{targetId}/!detach/contact/{attachmentId}` | `operation--estimate--targetId---detach-contact--attachmentId--post` | Detach a contact. |  |
