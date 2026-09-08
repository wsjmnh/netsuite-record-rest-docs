# vendorReturnAuthorization

Browser tag `vendorReturnAuthorization` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/vendorReturnAuthorization`, instance `/vendorReturnAuthorization/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/vendorReturnAuthorization` | `operation--vendorReturnAuthorization-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/vendorReturnAuthorization` | `operation--vendorReturnAuthorization-get` | Get list of records. |  | 200 OK → `vendorReturnAuthorizationCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/vendorReturnAuthorization` | `operation--vendorReturnAuthorization-patch` | Update records. | `vendorReturnAuthorizationCollection` | 202 Accepted; default → `nsError` |
| POST | `/vendorReturnAuthorization` | `operation--vendorReturnAuthorization-post` | Insert record. | `vendorReturnAuthorization` | 200 OK → `vendorReturnAuthorization`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/vendorReturnAuthorization` | `operation--vendorReturnAuthorization-put` | Insert or update records. | `vendorReturnAuthorizationCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/vendorReturnAuthorization/{id}` | `operation--vendorReturnAuthorization--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/vendorReturnAuthorization/{id}` | `operation--vendorReturnAuthorization--id--get` | Get record. |  | 200 OK → `vendorReturnAuthorization`; 202 Accepted; default → `nsError` |
| PATCH | `/vendorReturnAuthorization/{id}` | `operation--vendorReturnAuthorization--id--patch` | Update record. | `vendorReturnAuthorization` | 200 OK → `vendorReturnAuthorization`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/vendorReturnAuthorization/{id}` | `operation--vendorReturnAuthorization--id--put` | Insert or update record. | `vendorReturnAuthorization` | 202 Accepted; 204 No Content; default → `nsError` |
| POST | `/vendorReturnAuthorization/{id}/!transform/itemFulfillment` | `operation--vendorReturnAuthorization--id---transform-itemFulfillment-post` | Transform to itemFulfillment. | `itemFulfillment` | 200 OK → `vendorReturnAuthorization`; 202 Accepted; 204 No Content → `itemFulfillment`; default → `nsError` |
| POST | `/vendorReturnAuthorization/{id}/!transform/vendorCredit` | `operation--vendorReturnAuthorization--id---transform-vendorCredit-post` | Transform to vendorCredit. | `vendorCredit` | 200 OK → `vendorReturnAuthorization`; 202 Accepted; 204 No Content → `vendorCredit`; default → `nsError` |
| POST | `/vendorReturnAuthorization/{targetId}/!attach/contact/{attachmentId}` | `operation--vendorReturnAuthorization--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` | 202 Accepted; 204 No Content |
| POST | `/vendorReturnAuthorization/{targetId}/!detach/contact/{attachmentId}` | `operation--vendorReturnAuthorization--targetId---detach-contact--attachmentId--post` | Detach a contact. |  | 202 Accepted; 204 No Content |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--vendorReturnAuthorization-delete` | DELETE `/vendorReturnAuthorization` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorReturnAuthorization-get` | GET `/vendorReturnAuthorization` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorReturnAuthorization-patch` | PATCH `/vendorReturnAuthorization` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorReturnAuthorization-post` | POST `/vendorReturnAuthorization` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--vendorReturnAuthorization-put` | PUT `/vendorReturnAuthorization` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorReturnAuthorization--id--delete` | DELETE `/vendorReturnAuthorization/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorReturnAuthorization--id--get` | GET `/vendorReturnAuthorization/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorReturnAuthorization--id--patch` | PATCH `/vendorReturnAuthorization/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--vendorReturnAuthorization--id--put` | PUT `/vendorReturnAuthorization/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--vendorReturnAuthorization--id---transform-itemFulfillment-post` | POST `/vendorReturnAuthorization/{id}/!transform/itemFulfillment` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--vendorReturnAuthorization--id---transform-vendorCredit-post` | POST `/vendorReturnAuthorization/{id}/!transform/vendorCredit` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--vendorReturnAuthorization--targetId---attach-contact--attachmentId--post` | POST `/vendorReturnAuthorization/{targetId}/!attach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorReturnAuthorization--targetId---detach-contact--attachmentId--post` | POST `/vendorReturnAuthorization/{targetId}/!detach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |

## Inline request bodies

### `operation--vendorReturnAuthorization--targetId---attach-contact--attachmentId--post`

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `role` |  | object |  |  |  |  |
| `role.externalId` |  | string |  |  |  |  |
| `role.id` |  | integer | int32 |  |  |  |


## Schema refs

Definitions owned by this record (property tables): [vendorReturnAuthorization schemas](../schemas/vendorReturnAuthorization.md).

| Definition | Role |
| --- | --- |
| [`vendorReturnAuthorization`](../schemas/vendorReturnAuthorization.md#vendorreturnauthorization) | record body |
| [`vendorReturnAuthorization-accountingBookDetailCollection`](../schemas/vendorReturnAuthorization.md#vendorreturnauthorization-accountingbookdetailcollection) | sublist/collection |
| [`vendorReturnAuthorization-accountingBookDetailElement`](../schemas/vendorReturnAuthorization.md#vendorreturnauthorization-accountingbookdetailelement) | sublist/element |
| [`vendorReturnAuthorization-billingAddress`](../schemas/vendorReturnAuthorization.md#vendorreturnauthorization-billingaddress) | related |
| [`vendorReturnAuthorization-expenseCollection`](../schemas/vendorReturnAuthorization.md#vendorreturnauthorization-expensecollection) | sublist/collection |
| [`vendorReturnAuthorization-expenseElement`](../schemas/vendorReturnAuthorization.md#vendorreturnauthorization-expenseelement) | sublist/element |
| [`vendorReturnAuthorization-item-inventoryDetail`](../schemas/vendorReturnAuthorization.md#vendorreturnauthorization-item-inventorydetail) | related |
| [`vendorReturnAuthorization-item-inventoryDetail-inventoryAssignmentCollection`](../schemas/vendorReturnAuthorization.md#vendorreturnauthorization-item-inventorydetail-inventoryassignmentcollection) | sublist/collection |
| [`vendorReturnAuthorization-item-inventoryDetail-inventoryAssignmentElement`](../schemas/vendorReturnAuthorization.md#vendorreturnauthorization-item-inventorydetail-inventoryassignmentelement) | sublist/element |
| [`vendorReturnAuthorization-itemCollection`](../schemas/vendorReturnAuthorization.md#vendorreturnauthorization-itemcollection) | sublist/collection |
| [`vendorReturnAuthorization-itemElement`](../schemas/vendorReturnAuthorization.md#vendorreturnauthorization-itemelement) | sublist/element |
| [`vendorReturnAuthorization-taxDetailsCollection`](../schemas/vendorReturnAuthorization.md#vendorreturnauthorization-taxdetailscollection) | sublist/collection |
| [`vendorReturnAuthorization-taxDetailsElement`](../schemas/vendorReturnAuthorization.md#vendorreturnauthorization-taxdetailselement) | sublist/element |
| [`vendorReturnAuthorizationCollection`](../schemas/vendorReturnAuthorization.md#vendorreturnauthorizationcollection) | collection page |
| [`vendorReturnAuthorizationSelectOptions`](../schemas/vendorReturnAuthorization.md#vendorreturnauthorizationselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`itemFulfillment`](../schemas/itemFulfillment.md#itemfulfillment)
- [`nsError`](../schemas/ns.md#nserror)
- [`vendorCredit`](../schemas/vendorCredit.md#vendorcredit)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`vendorReturnAuthorization-accountingBookDetailCollection`](../schemas/vendorReturnAuthorization.md#vendorreturnauthorization-accountingbookdetailcollection) | [`vendorReturnAuthorization-accountingBookDetailElement`](../schemas/vendorReturnAuthorization.md#vendorreturnauthorization-accountingbookdetailelement) |
| `expense` | [`vendorReturnAuthorization-expenseCollection`](../schemas/vendorReturnAuthorization.md#vendorreturnauthorization-expensecollection) | [`vendorReturnAuthorization-expenseElement`](../schemas/vendorReturnAuthorization.md#vendorreturnauthorization-expenseelement) |
| `item` | [`vendorReturnAuthorization-itemCollection`](../schemas/vendorReturnAuthorization.md#vendorreturnauthorization-itemcollection) | [`vendorReturnAuthorization-itemElement`](../schemas/vendorReturnAuthorization.md#vendorreturnauthorization-itemelement) |
| `taxDetails` | [`vendorReturnAuthorization-taxDetailsCollection`](../schemas/vendorReturnAuthorization.md#vendorreturnauthorization-taxdetailscollection) | [`vendorReturnAuthorization-taxDetailsElement`](../schemas/vendorReturnAuthorization.md#vendorreturnauthorization-taxdetailselement) |

## Transforms

| Method | Path | Operation ID | Summary | Target | Request body |
| --- | --- | --- | --- | --- | --- |
| POST | `/vendorReturnAuthorization/{id}/!transform/itemFulfillment` | `operation--vendorReturnAuthorization--id---transform-itemFulfillment-post` | Transform to itemFulfillment. | `itemFulfillment` | `itemFulfillment` |
| POST | `/vendorReturnAuthorization/{id}/!transform/vendorCredit` | `operation--vendorReturnAuthorization--id---transform-vendorCredit-post` | Transform to vendorCredit. | `vendorCredit` | `vendorCredit` |

## Attach / detach

| Method | Path | Operation ID | Summary | Request body |
| --- | --- | --- | --- | --- |
| POST | `/vendorReturnAuthorization/{targetId}/!attach/contact/{attachmentId}` | `operation--vendorReturnAuthorization--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` |
| POST | `/vendorReturnAuthorization/{targetId}/!detach/contact/{attachmentId}` | `operation--vendorReturnAuthorization--targetId---detach-contact--attachmentId--post` | Detach a contact. |  |
