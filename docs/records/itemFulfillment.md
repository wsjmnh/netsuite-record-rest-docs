# itemFulfillment

Browser tag `itemFulfillment` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/itemFulfillment`, instance `/itemFulfillment/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/itemFulfillment` | `operation--itemFulfillment-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/itemFulfillment` | `operation--itemFulfillment-get` | Get list of records. |  | 200 OK → `itemFulfillmentCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/itemFulfillment` | `operation--itemFulfillment-patch` | Update records. | `itemFulfillmentCollection` | 202 Accepted; default → `nsError` |
| POST | `/itemFulfillment` | `operation--itemFulfillment-post` | Insert record. | `itemFulfillment` | 200 OK → `itemFulfillment`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/itemFulfillment` | `operation--itemFulfillment-put` | Insert or update records. | `itemFulfillmentCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/itemFulfillment/{id}` | `operation--itemFulfillment--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/itemFulfillment/{id}` | `operation--itemFulfillment--id--get` | Get record. |  | 200 OK → `itemFulfillment`; 202 Accepted; default → `nsError` |
| PATCH | `/itemFulfillment/{id}` | `operation--itemFulfillment--id--patch` | Update record. | `itemFulfillment` | 200 OK → `itemFulfillment`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/itemFulfillment/{id}` | `operation--itemFulfillment--id--put` | Insert or update record. | `itemFulfillment` | 202 Accepted; 204 No Content; default → `nsError` |
| POST | `/itemFulfillment/{targetId}/!attach/contact/{attachmentId}` | `operation--itemFulfillment--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` | 202 Accepted; 204 No Content |
| POST | `/itemFulfillment/{targetId}/!detach/contact/{attachmentId}` | `operation--itemFulfillment--targetId---detach-contact--attachmentId--post` | Detach a contact. |  | 202 Accepted; 204 No Content |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--itemFulfillment-delete` | DELETE `/itemFulfillment` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemFulfillment-get` | GET `/itemFulfillment` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemFulfillment-patch` | PATCH `/itemFulfillment` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemFulfillment-post` | POST `/itemFulfillment` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--itemFulfillment-put` | PUT `/itemFulfillment` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemFulfillment--id--delete` | DELETE `/itemFulfillment/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemFulfillment--id--get` | GET `/itemFulfillment/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemFulfillment--id--patch` | PATCH `/itemFulfillment/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--itemFulfillment--id--put` | PUT `/itemFulfillment/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--itemFulfillment--targetId---attach-contact--attachmentId--post` | POST `/itemFulfillment/{targetId}/!attach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemFulfillment--targetId---detach-contact--attachmentId--post` | POST `/itemFulfillment/{targetId}/!detach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |

## Inline request bodies

### `operation--itemFulfillment--targetId---attach-contact--attachmentId--post`

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `role` |  | object |  |  |  |  |
| `role.externalId` |  | string |  |  |  |  |
| `role.id` |  | integer | int32 |  |  |  |


## Schema refs

Definitions owned by this record (property tables): [itemFulfillment schemas](../schemas/itemFulfillment.md).

| Definition | Role |
| --- | --- |
| [`itemFulfillment`](../schemas/itemFulfillment.md#itemfulfillment) | record body |
| [`itemFulfillment-accountingBookDetailCollection`](../schemas/itemFulfillment.md#itemfulfillment-accountingbookdetailcollection) | sublist/collection |
| [`itemFulfillment-accountingBookDetailElement`](../schemas/itemFulfillment.md#itemfulfillment-accountingbookdetailelement) | sublist/element |
| [`itemFulfillment-appliedRulesCollection`](../schemas/itemFulfillment.md#itemfulfillment-appliedrulescollection) | sublist/collection |
| [`itemFulfillment-appliedRulesElement`](../schemas/itemFulfillment.md#itemfulfillment-appliedruleselement) | sublist/element |
| [`itemFulfillment-item-inventoryDetail`](../schemas/itemFulfillment.md#itemfulfillment-item-inventorydetail) | related |
| [`itemFulfillment-item-inventoryDetail-inventoryAssignmentCollection`](../schemas/itemFulfillment.md#itemfulfillment-item-inventorydetail-inventoryassignmentcollection) | sublist/collection |
| [`itemFulfillment-item-inventoryDetail-inventoryAssignmentElement`](../schemas/itemFulfillment.md#itemfulfillment-item-inventorydetail-inventoryassignmentelement) | sublist/element |
| [`itemFulfillment-itemCollection`](../schemas/itemFulfillment.md#itemfulfillment-itemcollection) | sublist/collection |
| [`itemFulfillment-itemElement`](../schemas/itemFulfillment.md#itemfulfillment-itemelement) | sublist/element |
| [`itemFulfillment-package-packageDetails`](../schemas/itemFulfillment.md#itemfulfillment-package-packagedetails) | related |
| [`itemFulfillment-packageCollection`](../schemas/itemFulfillment.md#itemfulfillment-packagecollection) | sublist/collection |
| [`itemFulfillment-packageElement`](../schemas/itemFulfillment.md#itemfulfillment-packageelement) | sublist/element |
| [`itemFulfillment-packageFedexCollection`](../schemas/itemFulfillment.md#itemfulfillment-packagefedexcollection) | sublist/collection |
| [`itemFulfillment-packageFedexElement`](../schemas/itemFulfillment.md#itemfulfillment-packagefedexelement) | sublist/element |
| [`itemFulfillment-packageUpsCollection`](../schemas/itemFulfillment.md#itemfulfillment-packageupscollection) | sublist/collection |
| [`itemFulfillment-packageUpsElement`](../schemas/itemFulfillment.md#itemfulfillment-packageupselement) | sublist/element |
| [`itemFulfillment-packageUspsCollection`](../schemas/itemFulfillment.md#itemfulfillment-packageuspscollection) | sublist/collection |
| [`itemFulfillment-packageUspsElement`](../schemas/itemFulfillment.md#itemfulfillment-packageuspselement) | sublist/element |
| [`itemFulfillment-returnShippingAddress`](../schemas/itemFulfillment.md#itemfulfillment-returnshippingaddress) | related |
| [`itemFulfillment-shipmentDetails`](../schemas/itemFulfillment.md#itemfulfillment-shipmentdetails) | related |
| [`itemFulfillment-shipmentPackageCollection`](../schemas/itemFulfillment.md#itemfulfillment-shipmentpackagecollection) | sublist/collection |
| [`itemFulfillment-shipmentPackageElement`](../schemas/itemFulfillment.md#itemfulfillment-shipmentpackageelement) | sublist/element |
| [`itemFulfillment-shippingAddress`](../schemas/itemFulfillment.md#itemfulfillment-shippingaddress) | related |
| [`itemFulfillmentCollection`](../schemas/itemFulfillment.md#itemfulfillmentcollection) | collection page |
| [`itemFulfillmentSelectOptions`](../schemas/itemFulfillment.md#itemfulfillmentselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`itemFulfillment-accountingBookDetailCollection`](../schemas/itemFulfillment.md#itemfulfillment-accountingbookdetailcollection) | [`itemFulfillment-accountingBookDetailElement`](../schemas/itemFulfillment.md#itemfulfillment-accountingbookdetailelement) |
| `appliedRules` | [`itemFulfillment-appliedRulesCollection`](../schemas/itemFulfillment.md#itemfulfillment-appliedrulescollection) | [`itemFulfillment-appliedRulesElement`](../schemas/itemFulfillment.md#itemfulfillment-appliedruleselement) |
| `item` | [`itemFulfillment-itemCollection`](../schemas/itemFulfillment.md#itemfulfillment-itemcollection) | [`itemFulfillment-itemElement`](../schemas/itemFulfillment.md#itemfulfillment-itemelement) |
| `package` | [`itemFulfillment-packageCollection`](../schemas/itemFulfillment.md#itemfulfillment-packagecollection) | [`itemFulfillment-packageElement`](../schemas/itemFulfillment.md#itemfulfillment-packageelement) |
| `packageFedex` | [`itemFulfillment-packageFedexCollection`](../schemas/itemFulfillment.md#itemfulfillment-packagefedexcollection) | [`itemFulfillment-packageFedexElement`](../schemas/itemFulfillment.md#itemfulfillment-packagefedexelement) |
| `packageUps` | [`itemFulfillment-packageUpsCollection`](../schemas/itemFulfillment.md#itemfulfillment-packageupscollection) | [`itemFulfillment-packageUpsElement`](../schemas/itemFulfillment.md#itemfulfillment-packageupselement) |
| `packageUsps` | [`itemFulfillment-packageUspsCollection`](../schemas/itemFulfillment.md#itemfulfillment-packageuspscollection) | [`itemFulfillment-packageUspsElement`](../schemas/itemFulfillment.md#itemfulfillment-packageuspselement) |
| `shipmentPackage` | [`itemFulfillment-shipmentPackageCollection`](../schemas/itemFulfillment.md#itemfulfillment-shipmentpackagecollection) | [`itemFulfillment-shipmentPackageElement`](../schemas/itemFulfillment.md#itemfulfillment-shipmentpackageelement) |

## Attach / detach

| Method | Path | Operation ID | Summary | Request body |
| --- | --- | --- | --- | --- |
| POST | `/itemFulfillment/{targetId}/!attach/contact/{attachmentId}` | `operation--itemFulfillment--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` |
| POST | `/itemFulfillment/{targetId}/!detach/contact/{attachmentId}` | `operation--itemFulfillment--targetId---detach-contact--attachmentId--post` | Detach a contact. |  |
