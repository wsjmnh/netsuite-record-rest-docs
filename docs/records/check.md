# check

Browser tag `check` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/check`, instance `/check/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/check` | `operation--check-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/check` | `operation--check-get` | Get list of records. |  | 200 OK → `checkCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/check` | `operation--check-patch` | Update records. | `checkCollection` | 202 Accepted; default → `nsError` |
| POST | `/check` | `operation--check-post` | Insert record. | `check` | 200 OK → `check`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/check` | `operation--check-put` | Insert or update records. | `checkCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/check/{id}` | `operation--check--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/check/{id}` | `operation--check--id--get` | Get record. |  | 200 OK → `check`; 202 Accepted; default → `nsError` |
| PATCH | `/check/{id}` | `operation--check--id--patch` | Update record. | `check` | 200 OK → `check`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/check/{id}` | `operation--check--id--put` | Insert or update record. | `check` | 202 Accepted; 204 No Content; default → `nsError` |
| POST | `/check/{targetId}/!attach/contact/{attachmentId}` | `operation--check--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` | 202 Accepted; 204 No Content |
| POST | `/check/{targetId}/!detach/contact/{attachmentId}` | `operation--check--targetId---detach-contact--attachmentId--post` | Detach a contact. |  | 202 Accepted; 204 No Content |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--check-delete` | DELETE `/check` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--check-get` | GET `/check` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--check-patch` | PATCH `/check` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--check-post` | POST `/check` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--check-put` | PUT `/check` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--check--id--delete` | DELETE `/check/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--check--id--get` | GET `/check/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--check--id--patch` | PATCH `/check/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--check--id--put` | PUT `/check/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--check--targetId---attach-contact--attachmentId--post` | POST `/check/{targetId}/!attach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--check--targetId---detach-contact--attachmentId--post` | POST `/check/{targetId}/!detach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |

## Inline request bodies

### `operation--check--targetId---attach-contact--attachmentId--post`

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `role` |  | object |  |  |  |  |
| `role.externalId` |  | string |  |  |  |  |
| `role.id` |  | integer | int32 |  |  |  |


## Schema refs

Definitions owned by this record (property tables): [check schemas](../schemas/check.md).

| Definition | Role |
| --- | --- |
| [`check`](../schemas/check.md#check) | record body |
| [`check-accountingBookDetailCollection`](../schemas/check.md#check-accountingbookdetailcollection) | sublist/collection |
| [`check-accountingBookDetailElement`](../schemas/check.md#check-accountingbookdetailelement) | sublist/element |
| [`check-expenseCollection`](../schemas/check.md#check-expensecollection) | sublist/collection |
| [`check-expenseElement`](../schemas/check.md#check-expenseelement) | sublist/element |
| [`check-item-inventoryDetail`](../schemas/check.md#check-item-inventorydetail) | related |
| [`check-item-inventoryDetail-inventoryAssignmentCollection`](../schemas/check.md#check-item-inventorydetail-inventoryassignmentcollection) | sublist/collection |
| [`check-item-inventoryDetail-inventoryAssignmentElement`](../schemas/check.md#check-item-inventorydetail-inventoryassignmentelement) | sublist/element |
| [`check-item-landedCost`](../schemas/check.md#check-item-landedcost) | related |
| [`check-item-landedCost-landedCostDataCollection`](../schemas/check.md#check-item-landedcost-landedcostdatacollection) | sublist/collection |
| [`check-item-landedCost-landedCostDataElement`](../schemas/check.md#check-item-landedcost-landedcostdataelement) | sublist/element |
| [`check-itemCollection`](../schemas/check.md#check-itemcollection) | sublist/collection |
| [`check-itemElement`](../schemas/check.md#check-itemelement) | sublist/element |
| [`check-landedCostsCollection`](../schemas/check.md#check-landedcostscollection) | sublist/collection |
| [`check-landedCostsElement`](../schemas/check.md#check-landedcostselement) | sublist/element |
| [`check-payeeAddress`](../schemas/check.md#check-payeeaddress) | related |
| [`checkCollection`](../schemas/check.md#checkcollection) | collection page |
| [`checkSelectOptions`](../schemas/check.md#checkselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`check-accountingBookDetailCollection`](../schemas/check.md#check-accountingbookdetailcollection) | [`check-accountingBookDetailElement`](../schemas/check.md#check-accountingbookdetailelement) |
| `expense` | [`check-expenseCollection`](../schemas/check.md#check-expensecollection) | [`check-expenseElement`](../schemas/check.md#check-expenseelement) |
| `item` | [`check-itemCollection`](../schemas/check.md#check-itemcollection) | [`check-itemElement`](../schemas/check.md#check-itemelement) |
| `landedCosts` | [`check-landedCostsCollection`](../schemas/check.md#check-landedcostscollection) | [`check-landedCostsElement`](../schemas/check.md#check-landedcostselement) |

## Attach / detach

| Method | Path | Operation ID | Summary | Request body |
| --- | --- | --- | --- | --- |
| POST | `/check/{targetId}/!attach/contact/{attachmentId}` | `operation--check--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` |
| POST | `/check/{targetId}/!detach/contact/{attachmentId}` | `operation--check--targetId---detach-contact--attachmentId--post` | Detach a contact. |  |
