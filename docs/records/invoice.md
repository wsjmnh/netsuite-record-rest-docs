# invoice

Browser tag `invoice` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/invoice`, instance `/invoice/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/invoice` | `operation--invoice-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/invoice` | `operation--invoice-get` | Get list of records. |  | 200 OK → `invoiceCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/invoice` | `operation--invoice-patch` | Update records. | `invoiceCollection` | 202 Accepted; default → `nsError` |
| POST | `/invoice` | `operation--invoice-post` | Insert record. | `invoice` | 200 OK → `invoice`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/invoice` | `operation--invoice-put` | Insert or update records. | `invoiceCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/invoice/{id}` | `operation--invoice--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/invoice/{id}` | `operation--invoice--id--get` | Get record. |  | 200 OK → `invoice`; 202 Accepted; default → `nsError` |
| PATCH | `/invoice/{id}` | `operation--invoice--id--patch` | Update record. | `invoice` | 200 OK → `invoice`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/invoice/{id}` | `operation--invoice--id--put` | Insert or update record. | `invoice` | 202 Accepted; 204 No Content; default → `nsError` |
| POST | `/invoice/{id}/!transform/creditMemo` | `operation--invoice--id---transform-creditMemo-post` | Transform to creditMemo. | `creditMemo` | 200 OK → `invoice`; 202 Accepted; 204 No Content → `creditMemo`; default → `nsError` |
| POST | `/invoice/{id}/!transform/customerPayment` | `operation--invoice--id---transform-customerPayment-post` | Transform to customerPayment. | `customerPayment` | 200 OK → `invoice`; 202 Accepted; 204 No Content → `customerPayment`; default → `nsError` |
| POST | `/invoice/{id}/!transform/returnAuthorization` | `operation--invoice--id---transform-returnAuthorization-post` | Transform to returnAuthorization. | `returnAuthorization` | 200 OK → `invoice`; 202 Accepted; 204 No Content → `returnAuthorization`; default → `nsError` |
| POST | `/invoice/{targetId}/!attach/contact/{attachmentId}` | `operation--invoice--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` | 202 Accepted; 204 No Content |
| POST | `/invoice/{targetId}/!detach/contact/{attachmentId}` | `operation--invoice--targetId---detach-contact--attachmentId--post` | Detach a contact. |  | 202 Accepted; 204 No Content |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--invoice-delete` | DELETE `/invoice` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--invoice-get` | GET `/invoice` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--invoice-patch` | PATCH `/invoice` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--invoice-post` | POST `/invoice` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--invoice-put` | PUT `/invoice` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--invoice--id--delete` | DELETE `/invoice/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--invoice--id--get` | GET `/invoice/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--invoice--id--patch` | PATCH `/invoice/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--invoice--id--put` | PUT `/invoice/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--invoice--id---transform-creditMemo-post` | POST `/invoice/{id}/!transform/creditMemo` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--invoice--id---transform-customerPayment-post` | POST `/invoice/{id}/!transform/customerPayment` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--invoice--id---transform-returnAuthorization-post` | POST `/invoice/{id}/!transform/returnAuthorization` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--invoice--targetId---attach-contact--attachmentId--post` | POST `/invoice/{targetId}/!attach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--invoice--targetId---detach-contact--attachmentId--post` | POST `/invoice/{targetId}/!detach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |

## Inline request bodies

### `operation--invoice--targetId---attach-contact--attachmentId--post`

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `role` |  | object |  |  |  |  |
| `role.externalId` |  | string |  |  |  |  |
| `role.id` |  | integer | int32 |  |  |  |


## Schema refs

Definitions owned by this record (property tables): [invoice schemas](../schemas/invoice.md).

| Definition | Role |
| --- | --- |
| [`invoice`](../schemas/invoice.md#invoice) | record body |
| [`invoice-accountingBookDetailCollection`](../schemas/invoice.md#invoice-accountingbookdetailcollection) | sublist/collection |
| [`invoice-accountingBookDetailElement`](../schemas/invoice.md#invoice-accountingbookdetailelement) | sublist/element |
| [`invoice-appliedRulesCollection`](../schemas/invoice.md#invoice-appliedrulescollection) | sublist/collection |
| [`invoice-appliedRulesElement`](../schemas/invoice.md#invoice-appliedruleselement) | sublist/element |
| [`invoice-billingAddress`](../schemas/invoice.md#invoice-billingaddress) | related |
| [`invoice-expCostCollection`](../schemas/invoice.md#invoice-expcostcollection) | sublist/collection |
| [`invoice-expCostElement`](../schemas/invoice.md#invoice-expcostelement) | sublist/element |
| [`invoice-giftCertRedemptionCollection`](../schemas/invoice.md#invoice-giftcertredemptioncollection) | sublist/collection |
| [`invoice-giftCertRedemptionElement`](../schemas/invoice.md#invoice-giftcertredemptionelement) | sublist/element |
| [`invoice-installmentCollection`](../schemas/invoice.md#invoice-installmentcollection) | sublist/collection |
| [`invoice-installmentElement`](../schemas/invoice.md#invoice-installmentelement) | sublist/element |
| [`invoice-item-inventoryDetail`](../schemas/invoice.md#invoice-item-inventorydetail) | related |
| [`invoice-item-inventoryDetail-inventoryAssignmentCollection`](../schemas/invoice.md#invoice-item-inventorydetail-inventoryassignmentcollection) | sublist/collection |
| [`invoice-item-inventoryDetail-inventoryAssignmentElement`](../schemas/invoice.md#invoice-item-inventorydetail-inventoryassignmentelement) | sublist/element |
| [`invoice-itemCollection`](../schemas/invoice.md#invoice-itemcollection) | sublist/collection |
| [`invoice-itemCost-inventoryDetail`](../schemas/invoice.md#invoice-itemcost-inventorydetail) | related |
| [`invoice-itemCost-inventoryDetail-inventoryAssignmentCollection`](../schemas/invoice.md#invoice-itemcost-inventorydetail-inventoryassignmentcollection) | sublist/collection |
| [`invoice-itemCost-inventoryDetail-inventoryAssignmentElement`](../schemas/invoice.md#invoice-itemcost-inventorydetail-inventoryassignmentelement) | sublist/element |
| [`invoice-itemCostCollection`](../schemas/invoice.md#invoice-itemcostcollection) | sublist/collection |
| [`invoice-itemCostElement`](../schemas/invoice.md#invoice-itemcostelement) | sublist/element |
| [`invoice-itemElement`](../schemas/invoice.md#invoice-itemelement) | sublist/element |
| [`invoice-partnersCollection`](../schemas/invoice.md#invoice-partnerscollection) | sublist/collection |
| [`invoice-partnersElement`](../schemas/invoice.md#invoice-partnerselement) | sublist/element |
| [`invoice-promotionsCollection`](../schemas/invoice.md#invoice-promotionscollection) | sublist/collection |
| [`invoice-promotionsElement`](../schemas/invoice.md#invoice-promotionselement) | sublist/element |
| [`invoice-salesTeamCollection`](../schemas/invoice.md#invoice-salesteamcollection) | sublist/collection |
| [`invoice-salesTeamElement`](../schemas/invoice.md#invoice-salesteamelement) | sublist/element |
| [`invoice-shipGroupCollection`](../schemas/invoice.md#invoice-shipgroupcollection) | sublist/collection |
| [`invoice-shipGroupElement`](../schemas/invoice.md#invoice-shipgroupelement) | sublist/element |
| [`invoice-shippingAddress`](../schemas/invoice.md#invoice-shippingaddress) | related |
| [`invoice-taxDetailsCollection`](../schemas/invoice.md#invoice-taxdetailscollection) | sublist/collection |
| [`invoice-taxDetailsElement`](../schemas/invoice.md#invoice-taxdetailselement) | sublist/element |
| [`invoice-timeCollection`](../schemas/invoice.md#invoice-timecollection) | sublist/collection |
| [`invoice-timeElement`](../schemas/invoice.md#invoice-timeelement) | sublist/element |
| [`invoiceCollection`](../schemas/invoice.md#invoicecollection) | collection page |
| [`invoiceSelectOptions`](../schemas/invoice.md#invoiceselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`creditMemo`](../schemas/creditMemo.md#creditmemo)
- [`customerPayment`](../schemas/customerPayment.md#customerpayment)
- [`nsError`](../schemas/ns.md#nserror)
- [`returnAuthorization`](../schemas/returnAuthorization.md#returnauthorization)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`invoice-accountingBookDetailCollection`](../schemas/invoice.md#invoice-accountingbookdetailcollection) | [`invoice-accountingBookDetailElement`](../schemas/invoice.md#invoice-accountingbookdetailelement) |
| `appliedRules` | [`invoice-appliedRulesCollection`](../schemas/invoice.md#invoice-appliedrulescollection) | [`invoice-appliedRulesElement`](../schemas/invoice.md#invoice-appliedruleselement) |
| `expCost` | [`invoice-expCostCollection`](../schemas/invoice.md#invoice-expcostcollection) | [`invoice-expCostElement`](../schemas/invoice.md#invoice-expcostelement) |
| `giftCertRedemption` | [`invoice-giftCertRedemptionCollection`](../schemas/invoice.md#invoice-giftcertredemptioncollection) | [`invoice-giftCertRedemptionElement`](../schemas/invoice.md#invoice-giftcertredemptionelement) |
| `installment` | [`invoice-installmentCollection`](../schemas/invoice.md#invoice-installmentcollection) | [`invoice-installmentElement`](../schemas/invoice.md#invoice-installmentelement) |
| `item` | [`invoice-itemCollection`](../schemas/invoice.md#invoice-itemcollection) | [`invoice-itemElement`](../schemas/invoice.md#invoice-itemelement) |
| `itemCost` | [`invoice-itemCostCollection`](../schemas/invoice.md#invoice-itemcostcollection) | [`invoice-itemCostElement`](../schemas/invoice.md#invoice-itemcostelement) |
| `partners` | [`invoice-partnersCollection`](../schemas/invoice.md#invoice-partnerscollection) | [`invoice-partnersElement`](../schemas/invoice.md#invoice-partnerselement) |
| `promotions` | [`invoice-promotionsCollection`](../schemas/invoice.md#invoice-promotionscollection) | [`invoice-promotionsElement`](../schemas/invoice.md#invoice-promotionselement) |
| `salesTeam` | [`invoice-salesTeamCollection`](../schemas/invoice.md#invoice-salesteamcollection) | [`invoice-salesTeamElement`](../schemas/invoice.md#invoice-salesteamelement) |
| `shipGroup` | [`invoice-shipGroupCollection`](../schemas/invoice.md#invoice-shipgroupcollection) | [`invoice-shipGroupElement`](../schemas/invoice.md#invoice-shipgroupelement) |
| `taxDetails` | [`invoice-taxDetailsCollection`](../schemas/invoice.md#invoice-taxdetailscollection) | [`invoice-taxDetailsElement`](../schemas/invoice.md#invoice-taxdetailselement) |
| `time` | [`invoice-timeCollection`](../schemas/invoice.md#invoice-timecollection) | [`invoice-timeElement`](../schemas/invoice.md#invoice-timeelement) |

## Transforms

| Method | Path | Operation ID | Summary | Target | Request body |
| --- | --- | --- | --- | --- | --- |
| POST | `/invoice/{id}/!transform/creditMemo` | `operation--invoice--id---transform-creditMemo-post` | Transform to creditMemo. | `creditMemo` | `creditMemo` |
| POST | `/invoice/{id}/!transform/customerPayment` | `operation--invoice--id---transform-customerPayment-post` | Transform to customerPayment. | `customerPayment` | `customerPayment` |
| POST | `/invoice/{id}/!transform/returnAuthorization` | `operation--invoice--id---transform-returnAuthorization-post` | Transform to returnAuthorization. | `returnAuthorization` | `returnAuthorization` |

## Attach / detach

| Method | Path | Operation ID | Summary | Request body |
| --- | --- | --- | --- | --- |
| POST | `/invoice/{targetId}/!attach/contact/{attachmentId}` | `operation--invoice--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` |
| POST | `/invoice/{targetId}/!detach/contact/{attachmentId}` | `operation--invoice--targetId---detach-contact--attachmentId--post` | Detach a contact. |  |
