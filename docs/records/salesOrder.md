# salesOrder

Browser tag `salesOrder` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/salesOrder`, instance `/salesOrder/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/salesOrder` | `operation--salesOrder-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/salesOrder` | `operation--salesOrder-get` | Get list of records. |  | 200 OK → `salesOrderCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/salesOrder` | `operation--salesOrder-patch` | Update records. | `salesOrderCollection` | 202 Accepted; default → `nsError` |
| POST | `/salesOrder` | `operation--salesOrder-post` | Insert record. | `salesOrder` | 200 OK → `salesOrder`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/salesOrder` | `operation--salesOrder-put` | Insert or update records. | `salesOrderCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/salesOrder/{id}` | `operation--salesOrder--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/salesOrder/{id}` | `operation--salesOrder--id--get` | Get record. |  | 200 OK → `salesOrder`; 202 Accepted; default → `nsError` |
| PATCH | `/salesOrder/{id}` | `operation--salesOrder--id--patch` | Update record. | `salesOrder` | 200 OK → `salesOrder`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/salesOrder/{id}` | `operation--salesOrder--id--put` | Insert or update record. | `salesOrder` | 202 Accepted; 204 No Content; default → `nsError` |
| POST | `/salesOrder/{id}/!transform/cashSale` | `operation--salesOrder--id---transform-cashSale-post` | Transform to cashSale. | `cashSale` | 200 OK → `salesOrder`; 202 Accepted; 204 No Content → `cashSale`; default → `nsError` |
| POST | `/salesOrder/{id}/!transform/fulfillmentRequest` | `operation--salesOrder--id---transform-fulfillmentRequest-post` | Transform to fulfillmentRequest. | `fulfillmentRequest` | 200 OK → `salesOrder`; 202 Accepted; 204 No Content → `fulfillmentRequest`; default → `nsError` |
| POST | `/salesOrder/{id}/!transform/invoice` | `operation--salesOrder--id---transform-invoice-post` | Transform to invoice. | `invoice` | 200 OK → `salesOrder`; 202 Accepted; 204 No Content → `invoice`; default → `nsError` |
| POST | `/salesOrder/{id}/!transform/itemFulfillment` | `operation--salesOrder--id---transform-itemFulfillment-post` | Transform to itemFulfillment. | `itemFulfillment` | 200 OK → `salesOrder`; 202 Accepted; 204 No Content → `itemFulfillment`; default → `nsError` |
| POST | `/salesOrder/{id}/!transform/returnAuthorization` | `operation--salesOrder--id---transform-returnAuthorization-post` | Transform to returnAuthorization. | `returnAuthorization` | 200 OK → `salesOrder`; 202 Accepted; 204 No Content → `returnAuthorization`; default → `nsError` |
| POST | `/salesOrder/{targetId}/!attach/contact/{attachmentId}` | `operation--salesOrder--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` | 202 Accepted; 204 No Content |
| POST | `/salesOrder/{targetId}/!detach/contact/{attachmentId}` | `operation--salesOrder--targetId---detach-contact--attachmentId--post` | Detach a contact. |  | 202 Accepted; 204 No Content |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--salesOrder-delete` | DELETE `/salesOrder` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--salesOrder-get` | GET `/salesOrder` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--salesOrder-patch` | PATCH `/salesOrder` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--salesOrder-post` | POST `/salesOrder` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--salesOrder-put` | PUT `/salesOrder` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--salesOrder--id--delete` | DELETE `/salesOrder/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--salesOrder--id--get` | GET `/salesOrder/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--salesOrder--id--patch` | PATCH `/salesOrder/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--salesOrder--id--put` | PUT `/salesOrder/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--salesOrder--id---transform-cashSale-post` | POST `/salesOrder/{id}/!transform/cashSale` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--salesOrder--id---transform-fulfillmentRequest-post` | POST `/salesOrder/{id}/!transform/fulfillmentRequest` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--salesOrder--id---transform-invoice-post` | POST `/salesOrder/{id}/!transform/invoice` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--salesOrder--id---transform-itemFulfillment-post` | POST `/salesOrder/{id}/!transform/itemFulfillment` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--salesOrder--id---transform-returnAuthorization-post` | POST `/salesOrder/{id}/!transform/returnAuthorization` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--salesOrder--targetId---attach-contact--attachmentId--post` | POST `/salesOrder/{targetId}/!attach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--salesOrder--targetId---detach-contact--attachmentId--post` | POST `/salesOrder/{targetId}/!detach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |

## Inline request bodies

### `operation--salesOrder--targetId---attach-contact--attachmentId--post`

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `role` |  | object |  |  |  |  |
| `role.externalId` |  | string |  |  |  |  |
| `role.id` |  | integer | int32 |  |  |  |


## Schema refs

Definitions owned by this record (property tables): [salesOrder schemas](../schemas/salesOrder.md).

| Definition | Role |
| --- | --- |
| [`salesOrder`](../schemas/salesOrder.md#salesorder) | record body |
| [`salesOrder-accountingBookDetailCollection`](../schemas/salesOrder.md#salesorder-accountingbookdetailcollection) | sublist/collection |
| [`salesOrder-accountingBookDetailElement`](../schemas/salesOrder.md#salesorder-accountingbookdetailelement) | sublist/element |
| [`salesOrder-appliedRulesCollection`](../schemas/salesOrder.md#salesorder-appliedrulescollection) | sublist/collection |
| [`salesOrder-appliedRulesElement`](../schemas/salesOrder.md#salesorder-appliedruleselement) | sublist/element |
| [`salesOrder-billingAddress`](../schemas/salesOrder.md#salesorder-billingaddress) | related |
| [`salesOrder-giftCertRedemptionCollection`](../schemas/salesOrder.md#salesorder-giftcertredemptioncollection) | sublist/collection |
| [`salesOrder-giftCertRedemptionElement`](../schemas/salesOrder.md#salesorder-giftcertredemptionelement) | sublist/element |
| [`salesOrder-item-inventoryDetail`](../schemas/salesOrder.md#salesorder-item-inventorydetail) | related |
| [`salesOrder-item-inventoryDetail-inventoryAssignmentCollection`](../schemas/salesOrder.md#salesorder-item-inventorydetail-inventoryassignmentcollection) | sublist/collection |
| [`salesOrder-item-inventoryDetail-inventoryAssignmentElement`](../schemas/salesOrder.md#salesorder-item-inventorydetail-inventoryassignmentelement) | sublist/element |
| [`salesOrder-itemCollection`](../schemas/salesOrder.md#salesorder-itemcollection) | sublist/collection |
| [`salesOrder-itemElement`](../schemas/salesOrder.md#salesorder-itemelement) | sublist/element |
| [`salesOrder-partnersCollection`](../schemas/salesOrder.md#salesorder-partnerscollection) | sublist/collection |
| [`salesOrder-partnersElement`](../schemas/salesOrder.md#salesorder-partnerselement) | sublist/element |
| [`salesOrder-promotionsCollection`](../schemas/salesOrder.md#salesorder-promotionscollection) | sublist/collection |
| [`salesOrder-promotionsElement`](../schemas/salesOrder.md#salesorder-promotionselement) | sublist/element |
| [`salesOrder-salesTeamCollection`](../schemas/salesOrder.md#salesorder-salesteamcollection) | sublist/collection |
| [`salesOrder-salesTeamElement`](../schemas/salesOrder.md#salesorder-salesteamelement) | sublist/element |
| [`salesOrder-shipGroupCollection`](../schemas/salesOrder.md#salesorder-shipgroupcollection) | sublist/collection |
| [`salesOrder-shipGroupElement`](../schemas/salesOrder.md#salesorder-shipgroupelement) | sublist/element |
| [`salesOrder-shippingAddress`](../schemas/salesOrder.md#salesorder-shippingaddress) | related |
| [`salesOrder-taxDetailsCollection`](../schemas/salesOrder.md#salesorder-taxdetailscollection) | sublist/collection |
| [`salesOrder-taxDetailsElement`](../schemas/salesOrder.md#salesorder-taxdetailselement) | sublist/element |
| [`salesOrderCollection`](../schemas/salesOrder.md#salesordercollection) | collection page |
| [`salesOrderSelectOptions`](../schemas/salesOrder.md#salesorderselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`cashSale`](../schemas/cashSale.md#cashsale)
- [`fulfillmentRequest`](../schemas/fulfillmentRequest.md#fulfillmentrequest)
- [`invoice`](../schemas/invoice.md#invoice)
- [`itemFulfillment`](../schemas/itemFulfillment.md#itemfulfillment)
- [`nsError`](../schemas/ns.md#nserror)
- [`returnAuthorization`](../schemas/returnAuthorization.md#returnauthorization)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`salesOrder-accountingBookDetailCollection`](../schemas/salesOrder.md#salesorder-accountingbookdetailcollection) | [`salesOrder-accountingBookDetailElement`](../schemas/salesOrder.md#salesorder-accountingbookdetailelement) |
| `appliedRules` | [`salesOrder-appliedRulesCollection`](../schemas/salesOrder.md#salesorder-appliedrulescollection) | [`salesOrder-appliedRulesElement`](../schemas/salesOrder.md#salesorder-appliedruleselement) |
| `giftCertRedemption` | [`salesOrder-giftCertRedemptionCollection`](../schemas/salesOrder.md#salesorder-giftcertredemptioncollection) | [`salesOrder-giftCertRedemptionElement`](../schemas/salesOrder.md#salesorder-giftcertredemptionelement) |
| `item` | [`salesOrder-itemCollection`](../schemas/salesOrder.md#salesorder-itemcollection) | [`salesOrder-itemElement`](../schemas/salesOrder.md#salesorder-itemelement) |
| `partners` | [`salesOrder-partnersCollection`](../schemas/salesOrder.md#salesorder-partnerscollection) | [`salesOrder-partnersElement`](../schemas/salesOrder.md#salesorder-partnerselement) |
| `promotions` | [`salesOrder-promotionsCollection`](../schemas/salesOrder.md#salesorder-promotionscollection) | [`salesOrder-promotionsElement`](../schemas/salesOrder.md#salesorder-promotionselement) |
| `salesTeam` | [`salesOrder-salesTeamCollection`](../schemas/salesOrder.md#salesorder-salesteamcollection) | [`salesOrder-salesTeamElement`](../schemas/salesOrder.md#salesorder-salesteamelement) |
| `shipGroup` | [`salesOrder-shipGroupCollection`](../schemas/salesOrder.md#salesorder-shipgroupcollection) | [`salesOrder-shipGroupElement`](../schemas/salesOrder.md#salesorder-shipgroupelement) |
| `taxDetails` | [`salesOrder-taxDetailsCollection`](../schemas/salesOrder.md#salesorder-taxdetailscollection) | [`salesOrder-taxDetailsElement`](../schemas/salesOrder.md#salesorder-taxdetailselement) |

## Transforms

| Method | Path | Operation ID | Summary | Target | Request body |
| --- | --- | --- | --- | --- | --- |
| POST | `/salesOrder/{id}/!transform/cashSale` | `operation--salesOrder--id---transform-cashSale-post` | Transform to cashSale. | `cashSale` | `cashSale` |
| POST | `/salesOrder/{id}/!transform/fulfillmentRequest` | `operation--salesOrder--id---transform-fulfillmentRequest-post` | Transform to fulfillmentRequest. | `fulfillmentRequest` | `fulfillmentRequest` |
| POST | `/salesOrder/{id}/!transform/invoice` | `operation--salesOrder--id---transform-invoice-post` | Transform to invoice. | `invoice` | `invoice` |
| POST | `/salesOrder/{id}/!transform/itemFulfillment` | `operation--salesOrder--id---transform-itemFulfillment-post` | Transform to itemFulfillment. | `itemFulfillment` | `itemFulfillment` |
| POST | `/salesOrder/{id}/!transform/returnAuthorization` | `operation--salesOrder--id---transform-returnAuthorization-post` | Transform to returnAuthorization. | `returnAuthorization` | `returnAuthorization` |

## Attach / detach

| Method | Path | Operation ID | Summary | Request body |
| --- | --- | --- | --- | --- |
| POST | `/salesOrder/{targetId}/!attach/contact/{attachmentId}` | `operation--salesOrder--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` |
| POST | `/salesOrder/{targetId}/!detach/contact/{attachmentId}` | `operation--salesOrder--targetId---detach-contact--attachmentId--post` | Detach a contact. |  |
