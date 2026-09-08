# cashRefund

Browser tag `cashRefund` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/cashRefund`, instance `/cashRefund/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/cashRefund` | `operation--cashRefund-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/cashRefund` | `operation--cashRefund-get` | Get list of records. |  | 200 OK → `cashRefundCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/cashRefund` | `operation--cashRefund-patch` | Update records. | `cashRefundCollection` | 202 Accepted; default → `nsError` |
| POST | `/cashRefund` | `operation--cashRefund-post` | Insert record. | `cashRefund` | 200 OK → `cashRefund`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/cashRefund` | `operation--cashRefund-put` | Insert or update records. | `cashRefundCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/cashRefund/{id}` | `operation--cashRefund--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/cashRefund/{id}` | `operation--cashRefund--id--get` | Get record. |  | 200 OK → `cashRefund`; 202 Accepted; default → `nsError` |
| PATCH | `/cashRefund/{id}` | `operation--cashRefund--id--patch` | Update record. | `cashRefund` | 200 OK → `cashRefund`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/cashRefund/{id}` | `operation--cashRefund--id--put` | Insert or update record. | `cashRefund` | 202 Accepted; 204 No Content; default → `nsError` |
| POST | `/cashRefund/{id}/!transform/creditMemo` | `operation--cashRefund--id---transform-creditMemo-post` | Transform to creditMemo. | `creditMemo` | 200 OK → `cashRefund`; 202 Accepted; 204 No Content → `creditMemo`; default → `nsError` |
| POST | `/cashRefund/{targetId}/!attach/contact/{attachmentId}` | `operation--cashRefund--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` | 202 Accepted; 204 No Content |
| POST | `/cashRefund/{targetId}/!detach/contact/{attachmentId}` | `operation--cashRefund--targetId---detach-contact--attachmentId--post` | Detach a contact. |  | 202 Accepted; 204 No Content |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--cashRefund-delete` | DELETE `/cashRefund` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--cashRefund-get` | GET `/cashRefund` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--cashRefund-patch` | PATCH `/cashRefund` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--cashRefund-post` | POST `/cashRefund` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--cashRefund-put` | PUT `/cashRefund` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--cashRefund--id--delete` | DELETE `/cashRefund/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--cashRefund--id--get` | GET `/cashRefund/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--cashRefund--id--patch` | PATCH `/cashRefund/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--cashRefund--id--put` | PUT `/cashRefund/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--cashRefund--id---transform-creditMemo-post` | POST `/cashRefund/{id}/!transform/creditMemo` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--cashRefund--targetId---attach-contact--attachmentId--post` | POST `/cashRefund/{targetId}/!attach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--cashRefund--targetId---detach-contact--attachmentId--post` | POST `/cashRefund/{targetId}/!detach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |

## Inline request bodies

### `operation--cashRefund--targetId---attach-contact--attachmentId--post`

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `role` |  | object |  |  |  |  |
| `role.externalId` |  | string |  |  |  |  |
| `role.id` |  | integer | int32 |  |  |  |


## Schema refs

Definitions owned by this record (property tables): [cashRefund schemas](../schemas/cashRefund.md).

| Definition | Role |
| --- | --- |
| [`cashRefund`](../schemas/cashRefund.md#cashrefund) | record body |
| [`cashRefund-accountingBookDetailCollection`](../schemas/cashRefund.md#cashrefund-accountingbookdetailcollection) | sublist/collection |
| [`cashRefund-accountingBookDetailElement`](../schemas/cashRefund.md#cashrefund-accountingbookdetailelement) | sublist/element |
| [`cashRefund-appliedRulesCollection`](../schemas/cashRefund.md#cashrefund-appliedrulescollection) | sublist/collection |
| [`cashRefund-appliedRulesElement`](../schemas/cashRefund.md#cashrefund-appliedruleselement) | sublist/element |
| [`cashRefund-billingAddress`](../schemas/cashRefund.md#cashrefund-billingaddress) | related |
| [`cashRefund-item-inventoryDetail`](../schemas/cashRefund.md#cashrefund-item-inventorydetail) | related |
| [`cashRefund-item-inventoryDetail-inventoryAssignmentCollection`](../schemas/cashRefund.md#cashrefund-item-inventorydetail-inventoryassignmentcollection) | sublist/collection |
| [`cashRefund-item-inventoryDetail-inventoryAssignmentElement`](../schemas/cashRefund.md#cashrefund-item-inventorydetail-inventoryassignmentelement) | sublist/element |
| [`cashRefund-itemCollection`](../schemas/cashRefund.md#cashrefund-itemcollection) | sublist/collection |
| [`cashRefund-itemElement`](../schemas/cashRefund.md#cashrefund-itemelement) | sublist/element |
| [`cashRefund-partnersCollection`](../schemas/cashRefund.md#cashrefund-partnerscollection) | sublist/collection |
| [`cashRefund-partnersElement`](../schemas/cashRefund.md#cashrefund-partnerselement) | sublist/element |
| [`cashRefund-promotionsCollection`](../schemas/cashRefund.md#cashrefund-promotionscollection) | sublist/collection |
| [`cashRefund-promotionsElement`](../schemas/cashRefund.md#cashrefund-promotionselement) | sublist/element |
| [`cashRefund-salesTeamCollection`](../schemas/cashRefund.md#cashrefund-salesteamcollection) | sublist/collection |
| [`cashRefund-salesTeamElement`](../schemas/cashRefund.md#cashrefund-salesteamelement) | sublist/element |
| [`cashRefund-shippingAddress`](../schemas/cashRefund.md#cashrefund-shippingaddress) | related |
| [`cashRefund-taxDetailsCollection`](../schemas/cashRefund.md#cashrefund-taxdetailscollection) | sublist/collection |
| [`cashRefund-taxDetailsElement`](../schemas/cashRefund.md#cashrefund-taxdetailselement) | sublist/element |
| [`cashRefundCollection`](../schemas/cashRefund.md#cashrefundcollection) | collection page |
| [`cashRefundSelectOptions`](../schemas/cashRefund.md#cashrefundselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`creditMemo`](../schemas/creditMemo.md#creditmemo)
- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`cashRefund-accountingBookDetailCollection`](../schemas/cashRefund.md#cashrefund-accountingbookdetailcollection) | [`cashRefund-accountingBookDetailElement`](../schemas/cashRefund.md#cashrefund-accountingbookdetailelement) |
| `appliedRules` | [`cashRefund-appliedRulesCollection`](../schemas/cashRefund.md#cashrefund-appliedrulescollection) | [`cashRefund-appliedRulesElement`](../schemas/cashRefund.md#cashrefund-appliedruleselement) |
| `item` | [`cashRefund-itemCollection`](../schemas/cashRefund.md#cashrefund-itemcollection) | [`cashRefund-itemElement`](../schemas/cashRefund.md#cashrefund-itemelement) |
| `partners` | [`cashRefund-partnersCollection`](../schemas/cashRefund.md#cashrefund-partnerscollection) | [`cashRefund-partnersElement`](../schemas/cashRefund.md#cashrefund-partnerselement) |
| `promotions` | [`cashRefund-promotionsCollection`](../schemas/cashRefund.md#cashrefund-promotionscollection) | [`cashRefund-promotionsElement`](../schemas/cashRefund.md#cashrefund-promotionselement) |
| `salesTeam` | [`cashRefund-salesTeamCollection`](../schemas/cashRefund.md#cashrefund-salesteamcollection) | [`cashRefund-salesTeamElement`](../schemas/cashRefund.md#cashrefund-salesteamelement) |
| `taxDetails` | [`cashRefund-taxDetailsCollection`](../schemas/cashRefund.md#cashrefund-taxdetailscollection) | [`cashRefund-taxDetailsElement`](../schemas/cashRefund.md#cashrefund-taxdetailselement) |

## Transforms

| Method | Path | Operation ID | Summary | Target | Request body |
| --- | --- | --- | --- | --- | --- |
| POST | `/cashRefund/{id}/!transform/creditMemo` | `operation--cashRefund--id---transform-creditMemo-post` | Transform to creditMemo. | `creditMemo` | `creditMemo` |

## Attach / detach

| Method | Path | Operation ID | Summary | Request body |
| --- | --- | --- | --- | --- |
| POST | `/cashRefund/{targetId}/!attach/contact/{attachmentId}` | `operation--cashRefund--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` |
| POST | `/cashRefund/{targetId}/!detach/contact/{attachmentId}` | `operation--cashRefund--targetId---detach-contact--attachmentId--post` | Detach a contact. |  |
