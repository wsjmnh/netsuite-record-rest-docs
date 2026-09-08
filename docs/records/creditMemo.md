# creditMemo

Browser tag `creditMemo` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/creditMemo`, instance `/creditMemo/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/creditMemo` | `operation--creditMemo-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/creditMemo` | `operation--creditMemo-get` | Get list of records. |  | 200 OK → `creditMemoCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/creditMemo` | `operation--creditMemo-patch` | Update records. | `creditMemoCollection` | 202 Accepted; default → `nsError` |
| POST | `/creditMemo` | `operation--creditMemo-post` | Insert record. | `creditMemo` | 200 OK → `creditMemo`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/creditMemo` | `operation--creditMemo-put` | Insert or update records. | `creditMemoCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/creditMemo/{id}` | `operation--creditMemo--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/creditMemo/{id}` | `operation--creditMemo--id--get` | Get record. |  | 200 OK → `creditMemo`; 202 Accepted; default → `nsError` |
| PATCH | `/creditMemo/{id}` | `operation--creditMemo--id--patch` | Update record. | `creditMemo` | 200 OK → `creditMemo`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/creditMemo/{id}` | `operation--creditMemo--id--put` | Insert or update record. | `creditMemo` | 202 Accepted; 204 No Content; default → `nsError` |
| POST | `/creditMemo/{id}/!transform/customerRefund` | `operation--creditMemo--id---transform-customerRefund-post` | Transform to customerRefund. | `customerRefund` | 200 OK → `creditMemo`; 202 Accepted; 204 No Content → `customerRefund`; default → `nsError` |
| POST | `/creditMemo/{targetId}/!attach/contact/{attachmentId}` | `operation--creditMemo--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` | 202 Accepted; 204 No Content |
| POST | `/creditMemo/{targetId}/!detach/contact/{attachmentId}` | `operation--creditMemo--targetId---detach-contact--attachmentId--post` | Detach a contact. |  | 202 Accepted; 204 No Content |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--creditMemo-delete` | DELETE `/creditMemo` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--creditMemo-get` | GET `/creditMemo` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--creditMemo-patch` | PATCH `/creditMemo` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--creditMemo-post` | POST `/creditMemo` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--creditMemo-put` | PUT `/creditMemo` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--creditMemo--id--delete` | DELETE `/creditMemo/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--creditMemo--id--get` | GET `/creditMemo/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--creditMemo--id--patch` | PATCH `/creditMemo/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--creditMemo--id--put` | PUT `/creditMemo/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--creditMemo--id---transform-customerRefund-post` | POST `/creditMemo/{id}/!transform/customerRefund` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--creditMemo--targetId---attach-contact--attachmentId--post` | POST `/creditMemo/{targetId}/!attach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--creditMemo--targetId---detach-contact--attachmentId--post` | POST `/creditMemo/{targetId}/!detach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |

## Inline request bodies

### `operation--creditMemo--targetId---attach-contact--attachmentId--post`

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `role` |  | object |  |  |  |  |
| `role.externalId` |  | string |  |  |  |  |
| `role.id` |  | integer | int32 |  |  |  |


## Schema refs

Definitions owned by this record (property tables): [creditMemo schemas](../schemas/creditMemo.md).

| Definition | Role |
| --- | --- |
| [`creditMemo`](../schemas/creditMemo.md#creditmemo) | record body |
| [`creditMemo-accountingBookDetailCollection`](../schemas/creditMemo.md#creditmemo-accountingbookdetailcollection) | sublist/collection |
| [`creditMemo-accountingBookDetailElement`](../schemas/creditMemo.md#creditmemo-accountingbookdetailelement) | sublist/element |
| [`creditMemo-appliedRulesCollection`](../schemas/creditMemo.md#creditmemo-appliedrulescollection) | sublist/collection |
| [`creditMemo-appliedRulesElement`](../schemas/creditMemo.md#creditmemo-appliedruleselement) | sublist/element |
| [`creditMemo-applyCollection`](../schemas/creditMemo.md#creditmemo-applycollection) | sublist/collection |
| [`creditMemo-applyElement`](../schemas/creditMemo.md#creditmemo-applyelement) | sublist/element |
| [`creditMemo-billingAddress`](../schemas/creditMemo.md#creditmemo-billingaddress) | related |
| [`creditMemo-item-inventoryDetail`](../schemas/creditMemo.md#creditmemo-item-inventorydetail) | related |
| [`creditMemo-item-inventoryDetail-inventoryAssignmentCollection`](../schemas/creditMemo.md#creditmemo-item-inventorydetail-inventoryassignmentcollection) | sublist/collection |
| [`creditMemo-item-inventoryDetail-inventoryAssignmentElement`](../schemas/creditMemo.md#creditmemo-item-inventorydetail-inventoryassignmentelement) | sublist/element |
| [`creditMemo-itemCollection`](../schemas/creditMemo.md#creditmemo-itemcollection) | sublist/collection |
| [`creditMemo-itemElement`](../schemas/creditMemo.md#creditmemo-itemelement) | sublist/element |
| [`creditMemo-partnersCollection`](../schemas/creditMemo.md#creditmemo-partnerscollection) | sublist/collection |
| [`creditMemo-partnersElement`](../schemas/creditMemo.md#creditmemo-partnerselement) | sublist/element |
| [`creditMemo-promotionsCollection`](../schemas/creditMemo.md#creditmemo-promotionscollection) | sublist/collection |
| [`creditMemo-promotionsElement`](../schemas/creditMemo.md#creditmemo-promotionselement) | sublist/element |
| [`creditMemo-salesTeamCollection`](../schemas/creditMemo.md#creditmemo-salesteamcollection) | sublist/collection |
| [`creditMemo-salesTeamElement`](../schemas/creditMemo.md#creditmemo-salesteamelement) | sublist/element |
| [`creditMemo-shipGroupCollection`](../schemas/creditMemo.md#creditmemo-shipgroupcollection) | sublist/collection |
| [`creditMemo-shipGroupElement`](../schemas/creditMemo.md#creditmemo-shipgroupelement) | sublist/element |
| [`creditMemo-shippingAddress`](../schemas/creditMemo.md#creditmemo-shippingaddress) | related |
| [`creditMemo-taxDetailsCollection`](../schemas/creditMemo.md#creditmemo-taxdetailscollection) | sublist/collection |
| [`creditMemo-taxDetailsElement`](../schemas/creditMemo.md#creditmemo-taxdetailselement) | sublist/element |
| [`creditMemoCollection`](../schemas/creditMemo.md#creditmemocollection) | collection page |
| [`creditMemoSelectOptions`](../schemas/creditMemo.md#creditmemoselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`customerRefund`](../schemas/customerRefund.md#customerrefund)
- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`creditMemo-accountingBookDetailCollection`](../schemas/creditMemo.md#creditmemo-accountingbookdetailcollection) | [`creditMemo-accountingBookDetailElement`](../schemas/creditMemo.md#creditmemo-accountingbookdetailelement) |
| `appliedRules` | [`creditMemo-appliedRulesCollection`](../schemas/creditMemo.md#creditmemo-appliedrulescollection) | [`creditMemo-appliedRulesElement`](../schemas/creditMemo.md#creditmemo-appliedruleselement) |
| `apply` | [`creditMemo-applyCollection`](../schemas/creditMemo.md#creditmemo-applycollection) | [`creditMemo-applyElement`](../schemas/creditMemo.md#creditmemo-applyelement) |
| `item` | [`creditMemo-itemCollection`](../schemas/creditMemo.md#creditmemo-itemcollection) | [`creditMemo-itemElement`](../schemas/creditMemo.md#creditmemo-itemelement) |
| `partners` | [`creditMemo-partnersCollection`](../schemas/creditMemo.md#creditmemo-partnerscollection) | [`creditMemo-partnersElement`](../schemas/creditMemo.md#creditmemo-partnerselement) |
| `promotions` | [`creditMemo-promotionsCollection`](../schemas/creditMemo.md#creditmemo-promotionscollection) | [`creditMemo-promotionsElement`](../schemas/creditMemo.md#creditmemo-promotionselement) |
| `salesTeam` | [`creditMemo-salesTeamCollection`](../schemas/creditMemo.md#creditmemo-salesteamcollection) | [`creditMemo-salesTeamElement`](../schemas/creditMemo.md#creditmemo-salesteamelement) |
| `shipGroup` | [`creditMemo-shipGroupCollection`](../schemas/creditMemo.md#creditmemo-shipgroupcollection) | [`creditMemo-shipGroupElement`](../schemas/creditMemo.md#creditmemo-shipgroupelement) |
| `taxDetails` | [`creditMemo-taxDetailsCollection`](../schemas/creditMemo.md#creditmemo-taxdetailscollection) | [`creditMemo-taxDetailsElement`](../schemas/creditMemo.md#creditmemo-taxdetailselement) |

## Transforms

| Method | Path | Operation ID | Summary | Target | Request body |
| --- | --- | --- | --- | --- | --- |
| POST | `/creditMemo/{id}/!transform/customerRefund` | `operation--creditMemo--id---transform-customerRefund-post` | Transform to customerRefund. | `customerRefund` | `customerRefund` |

## Attach / detach

| Method | Path | Operation ID | Summary | Request body |
| --- | --- | --- | --- | --- |
| POST | `/creditMemo/{targetId}/!attach/contact/{attachmentId}` | `operation--creditMemo--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` |
| POST | `/creditMemo/{targetId}/!detach/contact/{attachmentId}` | `operation--creditMemo--targetId---detach-contact--attachmentId--post` | Detach a contact. |  |
