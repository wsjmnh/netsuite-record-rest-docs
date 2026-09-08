# cashSale

Browser tag `cashSale` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/cashSale`, instance `/cashSale/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/cashSale` | `operation--cashSale-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/cashSale` | `operation--cashSale-get` | Get list of records. |  | 200 OK → `cashSaleCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/cashSale` | `operation--cashSale-patch` | Update records. | `cashSaleCollection` | 202 Accepted; default → `nsError` |
| POST | `/cashSale` | `operation--cashSale-post` | Insert record. | `cashSale` | 200 OK → `cashSale`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/cashSale` | `operation--cashSale-put` | Insert or update records. | `cashSaleCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/cashSale/{id}` | `operation--cashSale--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/cashSale/{id}` | `operation--cashSale--id--get` | Get record. |  | 200 OK → `cashSale`; 202 Accepted; default → `nsError` |
| PATCH | `/cashSale/{id}` | `operation--cashSale--id--patch` | Update record. | `cashSale` | 200 OK → `cashSale`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/cashSale/{id}` | `operation--cashSale--id--put` | Insert or update record. | `cashSale` | 202 Accepted; 204 No Content; default → `nsError` |
| POST | `/cashSale/{id}/!transform/cashRefund` | `operation--cashSale--id---transform-cashRefund-post` | Transform to cashRefund. | `cashRefund` | 200 OK → `cashSale`; 202 Accepted; 204 No Content → `cashRefund`; default → `nsError` |
| POST | `/cashSale/{id}/!transform/returnAuthorization` | `operation--cashSale--id---transform-returnAuthorization-post` | Transform to returnAuthorization. | `returnAuthorization` | 200 OK → `cashSale`; 202 Accepted; 204 No Content → `returnAuthorization`; default → `nsError` |
| POST | `/cashSale/{targetId}/!attach/contact/{attachmentId}` | `operation--cashSale--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` | 202 Accepted; 204 No Content |
| POST | `/cashSale/{targetId}/!detach/contact/{attachmentId}` | `operation--cashSale--targetId---detach-contact--attachmentId--post` | Detach a contact. |  | 202 Accepted; 204 No Content |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--cashSale-delete` | DELETE `/cashSale` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--cashSale-get` | GET `/cashSale` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--cashSale-patch` | PATCH `/cashSale` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--cashSale-post` | POST `/cashSale` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--cashSale-put` | PUT `/cashSale` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--cashSale--id--delete` | DELETE `/cashSale/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--cashSale--id--get` | GET `/cashSale/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--cashSale--id--patch` | PATCH `/cashSale/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--cashSale--id--put` | PUT `/cashSale/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--cashSale--id---transform-cashRefund-post` | POST `/cashSale/{id}/!transform/cashRefund` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--cashSale--id---transform-returnAuthorization-post` | POST `/cashSale/{id}/!transform/returnAuthorization` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--cashSale--targetId---attach-contact--attachmentId--post` | POST `/cashSale/{targetId}/!attach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--cashSale--targetId---detach-contact--attachmentId--post` | POST `/cashSale/{targetId}/!detach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |

## Inline request bodies

### `operation--cashSale--targetId---attach-contact--attachmentId--post`

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `role` |  | object |  |  |  |  |
| `role.externalId` |  | string |  |  |  |  |
| `role.id` |  | integer | int32 |  |  |  |


## Schema refs

Definitions owned by this record (property tables): [cashSale schemas](../schemas/cashSale.md).

| Definition | Role |
| --- | --- |
| [`cashSale`](../schemas/cashSale.md#cashsale) | record body |
| [`cashSale-accountingBookDetailCollection`](../schemas/cashSale.md#cashsale-accountingbookdetailcollection) | sublist/collection |
| [`cashSale-accountingBookDetailElement`](../schemas/cashSale.md#cashsale-accountingbookdetailelement) | sublist/element |
| [`cashSale-appliedRulesCollection`](../schemas/cashSale.md#cashsale-appliedrulescollection) | sublist/collection |
| [`cashSale-appliedRulesElement`](../schemas/cashSale.md#cashsale-appliedruleselement) | sublist/element |
| [`cashSale-billingAddress`](../schemas/cashSale.md#cashsale-billingaddress) | related |
| [`cashSale-expCostCollection`](../schemas/cashSale.md#cashsale-expcostcollection) | sublist/collection |
| [`cashSale-expCostElement`](../schemas/cashSale.md#cashsale-expcostelement) | sublist/element |
| [`cashSale-giftCertRedemptionCollection`](../schemas/cashSale.md#cashsale-giftcertredemptioncollection) | sublist/collection |
| [`cashSale-giftCertRedemptionElement`](../schemas/cashSale.md#cashsale-giftcertredemptionelement) | sublist/element |
| [`cashSale-item-inventoryDetail`](../schemas/cashSale.md#cashsale-item-inventorydetail) | related |
| [`cashSale-item-inventoryDetail-inventoryAssignmentCollection`](../schemas/cashSale.md#cashsale-item-inventorydetail-inventoryassignmentcollection) | sublist/collection |
| [`cashSale-item-inventoryDetail-inventoryAssignmentElement`](../schemas/cashSale.md#cashsale-item-inventorydetail-inventoryassignmentelement) | sublist/element |
| [`cashSale-itemCollection`](../schemas/cashSale.md#cashsale-itemcollection) | sublist/collection |
| [`cashSale-itemCost-inventoryDetail`](../schemas/cashSale.md#cashsale-itemcost-inventorydetail) | related |
| [`cashSale-itemCost-inventoryDetail-inventoryAssignmentCollection`](../schemas/cashSale.md#cashsale-itemcost-inventorydetail-inventoryassignmentcollection) | sublist/collection |
| [`cashSale-itemCost-inventoryDetail-inventoryAssignmentElement`](../schemas/cashSale.md#cashsale-itemcost-inventorydetail-inventoryassignmentelement) | sublist/element |
| [`cashSale-itemCostCollection`](../schemas/cashSale.md#cashsale-itemcostcollection) | sublist/collection |
| [`cashSale-itemCostElement`](../schemas/cashSale.md#cashsale-itemcostelement) | sublist/element |
| [`cashSale-itemElement`](../schemas/cashSale.md#cashsale-itemelement) | sublist/element |
| [`cashSale-partnersCollection`](../schemas/cashSale.md#cashsale-partnerscollection) | sublist/collection |
| [`cashSale-partnersElement`](../schemas/cashSale.md#cashsale-partnerselement) | sublist/element |
| [`cashSale-promotionsCollection`](../schemas/cashSale.md#cashsale-promotionscollection) | sublist/collection |
| [`cashSale-promotionsElement`](../schemas/cashSale.md#cashsale-promotionselement) | sublist/element |
| [`cashSale-salesTeamCollection`](../schemas/cashSale.md#cashsale-salesteamcollection) | sublist/collection |
| [`cashSale-salesTeamElement`](../schemas/cashSale.md#cashsale-salesteamelement) | sublist/element |
| [`cashSale-shipGroupCollection`](../schemas/cashSale.md#cashsale-shipgroupcollection) | sublist/collection |
| [`cashSale-shipGroupElement`](../schemas/cashSale.md#cashsale-shipgroupelement) | sublist/element |
| [`cashSale-shippingAddress`](../schemas/cashSale.md#cashsale-shippingaddress) | related |
| [`cashSale-taxDetailsCollection`](../schemas/cashSale.md#cashsale-taxdetailscollection) | sublist/collection |
| [`cashSale-taxDetailsElement`](../schemas/cashSale.md#cashsale-taxdetailselement) | sublist/element |
| [`cashSale-timeCollection`](../schemas/cashSale.md#cashsale-timecollection) | sublist/collection |
| [`cashSale-timeElement`](../schemas/cashSale.md#cashsale-timeelement) | sublist/element |
| [`cashSaleCollection`](../schemas/cashSale.md#cashsalecollection) | collection page |
| [`cashSaleSelectOptions`](../schemas/cashSale.md#cashsaleselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`cashRefund`](../schemas/cashRefund.md#cashrefund)
- [`nsError`](../schemas/ns.md#nserror)
- [`returnAuthorization`](../schemas/returnAuthorization.md#returnauthorization)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`cashSale-accountingBookDetailCollection`](../schemas/cashSale.md#cashsale-accountingbookdetailcollection) | [`cashSale-accountingBookDetailElement`](../schemas/cashSale.md#cashsale-accountingbookdetailelement) |
| `appliedRules` | [`cashSale-appliedRulesCollection`](../schemas/cashSale.md#cashsale-appliedrulescollection) | [`cashSale-appliedRulesElement`](../schemas/cashSale.md#cashsale-appliedruleselement) |
| `expCost` | [`cashSale-expCostCollection`](../schemas/cashSale.md#cashsale-expcostcollection) | [`cashSale-expCostElement`](../schemas/cashSale.md#cashsale-expcostelement) |
| `giftCertRedemption` | [`cashSale-giftCertRedemptionCollection`](../schemas/cashSale.md#cashsale-giftcertredemptioncollection) | [`cashSale-giftCertRedemptionElement`](../schemas/cashSale.md#cashsale-giftcertredemptionelement) |
| `item` | [`cashSale-itemCollection`](../schemas/cashSale.md#cashsale-itemcollection) | [`cashSale-itemElement`](../schemas/cashSale.md#cashsale-itemelement) |
| `itemCost` | [`cashSale-itemCostCollection`](../schemas/cashSale.md#cashsale-itemcostcollection) | [`cashSale-itemCostElement`](../schemas/cashSale.md#cashsale-itemcostelement) |
| `partners` | [`cashSale-partnersCollection`](../schemas/cashSale.md#cashsale-partnerscollection) | [`cashSale-partnersElement`](../schemas/cashSale.md#cashsale-partnerselement) |
| `promotions` | [`cashSale-promotionsCollection`](../schemas/cashSale.md#cashsale-promotionscollection) | [`cashSale-promotionsElement`](../schemas/cashSale.md#cashsale-promotionselement) |
| `salesTeam` | [`cashSale-salesTeamCollection`](../schemas/cashSale.md#cashsale-salesteamcollection) | [`cashSale-salesTeamElement`](../schemas/cashSale.md#cashsale-salesteamelement) |
| `shipGroup` | [`cashSale-shipGroupCollection`](../schemas/cashSale.md#cashsale-shipgroupcollection) | [`cashSale-shipGroupElement`](../schemas/cashSale.md#cashsale-shipgroupelement) |
| `taxDetails` | [`cashSale-taxDetailsCollection`](../schemas/cashSale.md#cashsale-taxdetailscollection) | [`cashSale-taxDetailsElement`](../schemas/cashSale.md#cashsale-taxdetailselement) |
| `time` | [`cashSale-timeCollection`](../schemas/cashSale.md#cashsale-timecollection) | [`cashSale-timeElement`](../schemas/cashSale.md#cashsale-timeelement) |

## Transforms

| Method | Path | Operation ID | Summary | Target | Request body |
| --- | --- | --- | --- | --- | --- |
| POST | `/cashSale/{id}/!transform/cashRefund` | `operation--cashSale--id---transform-cashRefund-post` | Transform to cashRefund. | `cashRefund` | `cashRefund` |
| POST | `/cashSale/{id}/!transform/returnAuthorization` | `operation--cashSale--id---transform-returnAuthorization-post` | Transform to returnAuthorization. | `returnAuthorization` | `returnAuthorization` |

## Attach / detach

| Method | Path | Operation ID | Summary | Request body |
| --- | --- | --- | --- | --- |
| POST | `/cashSale/{targetId}/!attach/contact/{attachmentId}` | `operation--cashSale--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` |
| POST | `/cashSale/{targetId}/!detach/contact/{attachmentId}` | `operation--cashSale--targetId---detach-contact--attachmentId--post` | Detach a contact. |  |
