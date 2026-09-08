# returnAuthorization

Browser tag `returnAuthorization` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/returnAuthorization`, instance `/returnAuthorization/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/returnAuthorization` | `operation--returnAuthorization-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/returnAuthorization` | `operation--returnAuthorization-get` | Get list of records. |  | 200 OK → `returnAuthorizationCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/returnAuthorization` | `operation--returnAuthorization-patch` | Update records. | `returnAuthorizationCollection` | 202 Accepted; default → `nsError` |
| POST | `/returnAuthorization` | `operation--returnAuthorization-post` | Insert record. | `returnAuthorization` | 200 OK → `returnAuthorization`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/returnAuthorization` | `operation--returnAuthorization-put` | Insert or update records. | `returnAuthorizationCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/returnAuthorization/{id}` | `operation--returnAuthorization--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/returnAuthorization/{id}` | `operation--returnAuthorization--id--get` | Get record. |  | 200 OK → `returnAuthorization`; 202 Accepted; default → `nsError` |
| PATCH | `/returnAuthorization/{id}` | `operation--returnAuthorization--id--patch` | Update record. | `returnAuthorization` | 200 OK → `returnAuthorization`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/returnAuthorization/{id}` | `operation--returnAuthorization--id--put` | Insert or update record. | `returnAuthorization` | 202 Accepted; 204 No Content; default → `nsError` |
| POST | `/returnAuthorization/{id}/!transform/cashRefund` | `operation--returnAuthorization--id---transform-cashRefund-post` | Transform to cashRefund. | `cashRefund` | 200 OK → `returnAuthorization`; 202 Accepted; 204 No Content → `cashRefund`; default → `nsError` |
| POST | `/returnAuthorization/{id}/!transform/creditMemo` | `operation--returnAuthorization--id---transform-creditMemo-post` | Transform to creditMemo. | `creditMemo` | 200 OK → `returnAuthorization`; 202 Accepted; 204 No Content → `creditMemo`; default → `nsError` |
| POST | `/returnAuthorization/{id}/!transform/itemReceipt` | `operation--returnAuthorization--id---transform-itemReceipt-post` | Transform to itemReceipt. | `itemReceipt` | 200 OK → `returnAuthorization`; 202 Accepted; 204 No Content → `itemReceipt`; default → `nsError` |
| POST | `/returnAuthorization/{targetId}/!attach/contact/{attachmentId}` | `operation--returnAuthorization--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` | 202 Accepted; 204 No Content |
| POST | `/returnAuthorization/{targetId}/!detach/contact/{attachmentId}` | `operation--returnAuthorization--targetId---detach-contact--attachmentId--post` | Detach a contact. |  | 202 Accepted; 204 No Content |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--returnAuthorization-delete` | DELETE `/returnAuthorization` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--returnAuthorization-get` | GET `/returnAuthorization` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--returnAuthorization-patch` | PATCH `/returnAuthorization` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--returnAuthorization-post` | POST `/returnAuthorization` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--returnAuthorization-put` | PUT `/returnAuthorization` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--returnAuthorization--id--delete` | DELETE `/returnAuthorization/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--returnAuthorization--id--get` | GET `/returnAuthorization/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--returnAuthorization--id--patch` | PATCH `/returnAuthorization/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--returnAuthorization--id--put` | PUT `/returnAuthorization/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--returnAuthorization--id---transform-cashRefund-post` | POST `/returnAuthorization/{id}/!transform/cashRefund` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--returnAuthorization--id---transform-creditMemo-post` | POST `/returnAuthorization/{id}/!transform/creditMemo` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--returnAuthorization--id---transform-itemReceipt-post` | POST `/returnAuthorization/{id}/!transform/itemReceipt` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--returnAuthorization--targetId---attach-contact--attachmentId--post` | POST `/returnAuthorization/{targetId}/!attach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--returnAuthorization--targetId---detach-contact--attachmentId--post` | POST `/returnAuthorization/{targetId}/!detach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |

## Inline request bodies

### `operation--returnAuthorization--targetId---attach-contact--attachmentId--post`

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `role` |  | object |  |  |  |  |
| `role.externalId` |  | string |  |  |  |  |
| `role.id` |  | integer | int32 |  |  |  |


## Schema refs

Definitions owned by this record (property tables): [returnAuthorization schemas](../schemas/returnAuthorization.md).

| Definition | Role |
| --- | --- |
| [`returnAuthorization`](../schemas/returnAuthorization.md#returnauthorization) | record body |
| [`returnAuthorization-accountingBookDetailCollection`](../schemas/returnAuthorization.md#returnauthorization-accountingbookdetailcollection) | sublist/collection |
| [`returnAuthorization-accountingBookDetailElement`](../schemas/returnAuthorization.md#returnauthorization-accountingbookdetailelement) | sublist/element |
| [`returnAuthorization-appliedRulesCollection`](../schemas/returnAuthorization.md#returnauthorization-appliedrulescollection) | sublist/collection |
| [`returnAuthorization-appliedRulesElement`](../schemas/returnAuthorization.md#returnauthorization-appliedruleselement) | sublist/element |
| [`returnAuthorization-billingAddress`](../schemas/returnAuthorization.md#returnauthorization-billingaddress) | related |
| [`returnAuthorization-item-inventoryDetail`](../schemas/returnAuthorization.md#returnauthorization-item-inventorydetail) | related |
| [`returnAuthorization-item-inventoryDetail-inventoryAssignmentCollection`](../schemas/returnAuthorization.md#returnauthorization-item-inventorydetail-inventoryassignmentcollection) | sublist/collection |
| [`returnAuthorization-item-inventoryDetail-inventoryAssignmentElement`](../schemas/returnAuthorization.md#returnauthorization-item-inventorydetail-inventoryassignmentelement) | sublist/element |
| [`returnAuthorization-itemCollection`](../schemas/returnAuthorization.md#returnauthorization-itemcollection) | sublist/collection |
| [`returnAuthorization-itemElement`](../schemas/returnAuthorization.md#returnauthorization-itemelement) | sublist/element |
| [`returnAuthorization-partnersCollection`](../schemas/returnAuthorization.md#returnauthorization-partnerscollection) | sublist/collection |
| [`returnAuthorization-partnersElement`](../schemas/returnAuthorization.md#returnauthorization-partnerselement) | sublist/element |
| [`returnAuthorization-promotionsCollection`](../schemas/returnAuthorization.md#returnauthorization-promotionscollection) | sublist/collection |
| [`returnAuthorization-promotionsElement`](../schemas/returnAuthorization.md#returnauthorization-promotionselement) | sublist/element |
| [`returnAuthorization-salesTeamCollection`](../schemas/returnAuthorization.md#returnauthorization-salesteamcollection) | sublist/collection |
| [`returnAuthorization-salesTeamElement`](../schemas/returnAuthorization.md#returnauthorization-salesteamelement) | sublist/element |
| [`returnAuthorization-shippingAddress`](../schemas/returnAuthorization.md#returnauthorization-shippingaddress) | related |
| [`returnAuthorization-taxDetailsCollection`](../schemas/returnAuthorization.md#returnauthorization-taxdetailscollection) | sublist/collection |
| [`returnAuthorization-taxDetailsElement`](../schemas/returnAuthorization.md#returnauthorization-taxdetailselement) | sublist/element |
| [`returnAuthorizationCollection`](../schemas/returnAuthorization.md#returnauthorizationcollection) | collection page |
| [`returnAuthorizationSelectOptions`](../schemas/returnAuthorization.md#returnauthorizationselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`cashRefund`](../schemas/cashRefund.md#cashrefund)
- [`creditMemo`](../schemas/creditMemo.md#creditmemo)
- [`itemReceipt`](../schemas/itemReceipt.md#itemreceipt)
- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`returnAuthorization-accountingBookDetailCollection`](../schemas/returnAuthorization.md#returnauthorization-accountingbookdetailcollection) | [`returnAuthorization-accountingBookDetailElement`](../schemas/returnAuthorization.md#returnauthorization-accountingbookdetailelement) |
| `appliedRules` | [`returnAuthorization-appliedRulesCollection`](../schemas/returnAuthorization.md#returnauthorization-appliedrulescollection) | [`returnAuthorization-appliedRulesElement`](../schemas/returnAuthorization.md#returnauthorization-appliedruleselement) |
| `item` | [`returnAuthorization-itemCollection`](../schemas/returnAuthorization.md#returnauthorization-itemcollection) | [`returnAuthorization-itemElement`](../schemas/returnAuthorization.md#returnauthorization-itemelement) |
| `partners` | [`returnAuthorization-partnersCollection`](../schemas/returnAuthorization.md#returnauthorization-partnerscollection) | [`returnAuthorization-partnersElement`](../schemas/returnAuthorization.md#returnauthorization-partnerselement) |
| `promotions` | [`returnAuthorization-promotionsCollection`](../schemas/returnAuthorization.md#returnauthorization-promotionscollection) | [`returnAuthorization-promotionsElement`](../schemas/returnAuthorization.md#returnauthorization-promotionselement) |
| `salesTeam` | [`returnAuthorization-salesTeamCollection`](../schemas/returnAuthorization.md#returnauthorization-salesteamcollection) | [`returnAuthorization-salesTeamElement`](../schemas/returnAuthorization.md#returnauthorization-salesteamelement) |
| `taxDetails` | [`returnAuthorization-taxDetailsCollection`](../schemas/returnAuthorization.md#returnauthorization-taxdetailscollection) | [`returnAuthorization-taxDetailsElement`](../schemas/returnAuthorization.md#returnauthorization-taxdetailselement) |

## Transforms

| Method | Path | Operation ID | Summary | Target | Request body |
| --- | --- | --- | --- | --- | --- |
| POST | `/returnAuthorization/{id}/!transform/cashRefund` | `operation--returnAuthorization--id---transform-cashRefund-post` | Transform to cashRefund. | `cashRefund` | `cashRefund` |
| POST | `/returnAuthorization/{id}/!transform/creditMemo` | `operation--returnAuthorization--id---transform-creditMemo-post` | Transform to creditMemo. | `creditMemo` | `creditMemo` |
| POST | `/returnAuthorization/{id}/!transform/itemReceipt` | `operation--returnAuthorization--id---transform-itemReceipt-post` | Transform to itemReceipt. | `itemReceipt` | `itemReceipt` |

## Attach / detach

| Method | Path | Operation ID | Summary | Request body |
| --- | --- | --- | --- | --- |
| POST | `/returnAuthorization/{targetId}/!attach/contact/{attachmentId}` | `operation--returnAuthorization--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` |
| POST | `/returnAuthorization/{targetId}/!detach/contact/{attachmentId}` | `operation--returnAuthorization--targetId---detach-contact--attachmentId--post` | Detach a contact. |  |
