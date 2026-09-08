# vendorBill

Browser tag `vendorBill` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/vendorBill`, instance `/vendorBill/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/vendorBill` | `operation--vendorBill-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/vendorBill` | `operation--vendorBill-get` | Get list of records. |  | 200 OK → `vendorBillCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/vendorBill` | `operation--vendorBill-patch` | Update records. | `vendorBillCollection` | 202 Accepted; default → `nsError` |
| POST | `/vendorBill` | `operation--vendorBill-post` | Insert record. | `vendorBill` | 200 OK → `vendorBill`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/vendorBill` | `operation--vendorBill-put` | Insert or update records. | `vendorBillCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/vendorBill/{id}` | `operation--vendorBill--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/vendorBill/{id}` | `operation--vendorBill--id--get` | Get record. |  | 200 OK → `vendorBill`; 202 Accepted; default → `nsError` |
| PATCH | `/vendorBill/{id}` | `operation--vendorBill--id--patch` | Update record. | `vendorBill` | 200 OK → `vendorBill`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/vendorBill/{id}` | `operation--vendorBill--id--put` | Insert or update record. | `vendorBill` | 202 Accepted; 204 No Content; default → `nsError` |
| POST | `/vendorBill/{id}/!transform/vendorCredit` | `operation--vendorBill--id---transform-vendorCredit-post` | Transform to vendorCredit. | `vendorCredit` | 200 OK → `vendorBill`; 202 Accepted; 204 No Content → `vendorCredit`; default → `nsError` |
| POST | `/vendorBill/{id}/!transform/vendorPayment` | `operation--vendorBill--id---transform-vendorPayment-post` | Transform to vendorPayment. | `vendorPayment` | 200 OK → `vendorBill`; 202 Accepted; 204 No Content → `vendorPayment`; default → `nsError` |
| POST | `/vendorBill/{id}/!transform/vendorReturnAuthorization` | `operation--vendorBill--id---transform-vendorReturnAuthorization-post` | Transform to vendorReturnAuthorization. | `vendorReturnAuthorization` | 200 OK → `vendorBill`; 202 Accepted; 204 No Content → `vendorReturnAuthorization`; default → `nsError` |
| POST | `/vendorBill/{targetId}/!attach/contact/{attachmentId}` | `operation--vendorBill--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` | 202 Accepted; 204 No Content |
| POST | `/vendorBill/{targetId}/!detach/contact/{attachmentId}` | `operation--vendorBill--targetId---detach-contact--attachmentId--post` | Detach a contact. |  | 202 Accepted; 204 No Content |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--vendorBill-delete` | DELETE `/vendorBill` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorBill-get` | GET `/vendorBill` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorBill-patch` | PATCH `/vendorBill` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorBill-post` | POST `/vendorBill` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--vendorBill-put` | PUT `/vendorBill` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorBill--id--delete` | DELETE `/vendorBill/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorBill--id--get` | GET `/vendorBill/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorBill--id--patch` | PATCH `/vendorBill/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--vendorBill--id--put` | PUT `/vendorBill/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--vendorBill--id---transform-vendorCredit-post` | POST `/vendorBill/{id}/!transform/vendorCredit` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--vendorBill--id---transform-vendorPayment-post` | POST `/vendorBill/{id}/!transform/vendorPayment` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--vendorBill--id---transform-vendorReturnAuthorization-post` | POST `/vendorBill/{id}/!transform/vendorReturnAuthorization` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--vendorBill--targetId---attach-contact--attachmentId--post` | POST `/vendorBill/{targetId}/!attach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorBill--targetId---detach-contact--attachmentId--post` | POST `/vendorBill/{targetId}/!detach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |

## Inline request bodies

### `operation--vendorBill--targetId---attach-contact--attachmentId--post`

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `role` |  | object |  |  |  |  |
| `role.externalId` |  | string |  |  |  |  |
| `role.id` |  | integer | int32 |  |  |  |


## Schema refs

Definitions owned by this record (property tables): [vendorBill schemas](../schemas/vendorBill.md).

| Definition | Role |
| --- | --- |
| [`vendorBill`](../schemas/vendorBill.md#vendorbill) | record body |
| [`vendorBill-accountingBookDetailCollection`](../schemas/vendorBill.md#vendorbill-accountingbookdetailcollection) | sublist/collection |
| [`vendorBill-accountingBookDetailElement`](../schemas/vendorBill.md#vendorbill-accountingbookdetailelement) | sublist/element |
| [`vendorBill-appliedRulesCollection`](../schemas/vendorBill.md#vendorbill-appliedrulescollection) | sublist/collection |
| [`vendorBill-appliedRulesElement`](../schemas/vendorBill.md#vendorbill-appliedruleselement) | sublist/element |
| [`vendorBill-billingAddress`](../schemas/vendorBill.md#vendorbill-billingaddress) | related |
| [`vendorBill-expenseCollection`](../schemas/vendorBill.md#vendorbill-expensecollection) | sublist/collection |
| [`vendorBill-expenseElement`](../schemas/vendorBill.md#vendorbill-expenseelement) | sublist/element |
| [`vendorBill-installmentCollection`](../schemas/vendorBill.md#vendorbill-installmentcollection) | sublist/collection |
| [`vendorBill-installmentElement`](../schemas/vendorBill.md#vendorbill-installmentelement) | sublist/element |
| [`vendorBill-item-inventoryDetail`](../schemas/vendorBill.md#vendorbill-item-inventorydetail) | related |
| [`vendorBill-item-inventoryDetail-inventoryAssignmentCollection`](../schemas/vendorBill.md#vendorbill-item-inventorydetail-inventoryassignmentcollection) | sublist/collection |
| [`vendorBill-item-inventoryDetail-inventoryAssignmentElement`](../schemas/vendorBill.md#vendorbill-item-inventorydetail-inventoryassignmentelement) | sublist/element |
| [`vendorBill-item-landedCost`](../schemas/vendorBill.md#vendorbill-item-landedcost) | related |
| [`vendorBill-item-landedCost-landedCostDataCollection`](../schemas/vendorBill.md#vendorbill-item-landedcost-landedcostdatacollection) | sublist/collection |
| [`vendorBill-item-landedCost-landedCostDataElement`](../schemas/vendorBill.md#vendorbill-item-landedcost-landedcostdataelement) | sublist/element |
| [`vendorBill-itemCollection`](../schemas/vendorBill.md#vendorbill-itemcollection) | sublist/collection |
| [`vendorBill-itemElement`](../schemas/vendorBill.md#vendorbill-itemelement) | sublist/element |
| [`vendorBill-landedCostsCollection`](../schemas/vendorBill.md#vendorbill-landedcostscollection) | sublist/collection |
| [`vendorBill-landedCostsElement`](../schemas/vendorBill.md#vendorbill-landedcostselement) | sublist/element |
| [`vendorBill-taxDetailsCollection`](../schemas/vendorBill.md#vendorbill-taxdetailscollection) | sublist/collection |
| [`vendorBill-taxDetailsElement`](../schemas/vendorBill.md#vendorbill-taxdetailselement) | sublist/element |
| [`vendorBillCollection`](../schemas/vendorBill.md#vendorbillcollection) | collection page |
| [`vendorBillSelectOptions`](../schemas/vendorBill.md#vendorbillselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)
- [`vendorCredit`](../schemas/vendorCredit.md#vendorcredit)
- [`vendorPayment`](../schemas/vendorPayment.md#vendorpayment)
- [`vendorReturnAuthorization`](../schemas/vendorReturnAuthorization.md#vendorreturnauthorization)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`vendorBill-accountingBookDetailCollection`](../schemas/vendorBill.md#vendorbill-accountingbookdetailcollection) | [`vendorBill-accountingBookDetailElement`](../schemas/vendorBill.md#vendorbill-accountingbookdetailelement) |
| `appliedRules` | [`vendorBill-appliedRulesCollection`](../schemas/vendorBill.md#vendorbill-appliedrulescollection) | [`vendorBill-appliedRulesElement`](../schemas/vendorBill.md#vendorbill-appliedruleselement) |
| `expense` | [`vendorBill-expenseCollection`](../schemas/vendorBill.md#vendorbill-expensecollection) | [`vendorBill-expenseElement`](../schemas/vendorBill.md#vendorbill-expenseelement) |
| `installment` | [`vendorBill-installmentCollection`](../schemas/vendorBill.md#vendorbill-installmentcollection) | [`vendorBill-installmentElement`](../schemas/vendorBill.md#vendorbill-installmentelement) |
| `item` | [`vendorBill-itemCollection`](../schemas/vendorBill.md#vendorbill-itemcollection) | [`vendorBill-itemElement`](../schemas/vendorBill.md#vendorbill-itemelement) |
| `landedCosts` | [`vendorBill-landedCostsCollection`](../schemas/vendorBill.md#vendorbill-landedcostscollection) | [`vendorBill-landedCostsElement`](../schemas/vendorBill.md#vendorbill-landedcostselement) |
| `taxDetails` | [`vendorBill-taxDetailsCollection`](../schemas/vendorBill.md#vendorbill-taxdetailscollection) | [`vendorBill-taxDetailsElement`](../schemas/vendorBill.md#vendorbill-taxdetailselement) |

## Transforms

| Method | Path | Operation ID | Summary | Target | Request body |
| --- | --- | --- | --- | --- | --- |
| POST | `/vendorBill/{id}/!transform/vendorCredit` | `operation--vendorBill--id---transform-vendorCredit-post` | Transform to vendorCredit. | `vendorCredit` | `vendorCredit` |
| POST | `/vendorBill/{id}/!transform/vendorPayment` | `operation--vendorBill--id---transform-vendorPayment-post` | Transform to vendorPayment. | `vendorPayment` | `vendorPayment` |
| POST | `/vendorBill/{id}/!transform/vendorReturnAuthorization` | `operation--vendorBill--id---transform-vendorReturnAuthorization-post` | Transform to vendorReturnAuthorization. | `vendorReturnAuthorization` | `vendorReturnAuthorization` |

## Attach / detach

| Method | Path | Operation ID | Summary | Request body |
| --- | --- | --- | --- | --- |
| POST | `/vendorBill/{targetId}/!attach/contact/{attachmentId}` | `operation--vendorBill--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` |
| POST | `/vendorBill/{targetId}/!detach/contact/{attachmentId}` | `operation--vendorBill--targetId---detach-contact--attachmentId--post` | Detach a contact. |  |
