# creditCardRefund

Browser tag `creditCardRefund` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/creditCardRefund`, instance `/creditCardRefund/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/creditCardRefund` | `operation--creditCardRefund-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/creditCardRefund` | `operation--creditCardRefund-get` | Get list of records. |  | 200 OK → `creditCardRefundCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/creditCardRefund` | `operation--creditCardRefund-patch` | Update records. | `creditCardRefundCollection` | 202 Accepted; default → `nsError` |
| POST | `/creditCardRefund` | `operation--creditCardRefund-post` | Insert record. | `creditCardRefund` | 200 OK → `creditCardRefund`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/creditCardRefund` | `operation--creditCardRefund-put` | Insert or update records. | `creditCardRefundCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/creditCardRefund/{id}` | `operation--creditCardRefund--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/creditCardRefund/{id}` | `operation--creditCardRefund--id--get` | Get record. |  | 200 OK → `creditCardRefund`; 202 Accepted; default → `nsError` |
| PATCH | `/creditCardRefund/{id}` | `operation--creditCardRefund--id--patch` | Update record. | `creditCardRefund` | 200 OK → `creditCardRefund`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/creditCardRefund/{id}` | `operation--creditCardRefund--id--put` | Insert or update record. | `creditCardRefund` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--creditCardRefund-delete` | DELETE `/creditCardRefund` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--creditCardRefund-get` | GET `/creditCardRefund` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--creditCardRefund-patch` | PATCH `/creditCardRefund` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--creditCardRefund-post` | POST `/creditCardRefund` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--creditCardRefund-put` | PUT `/creditCardRefund` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--creditCardRefund--id--delete` | DELETE `/creditCardRefund/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--creditCardRefund--id--get` | GET `/creditCardRefund/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--creditCardRefund--id--patch` | PATCH `/creditCardRefund/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--creditCardRefund--id--put` | PUT `/creditCardRefund/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [creditCardRefund schemas](../schemas/creditCardRefund.md).

| Definition | Role |
| --- | --- |
| [`creditCardRefund`](../schemas/creditCardRefund.md#creditcardrefund) | record body |
| [`creditCardRefund-accountingBookDetailCollection`](../schemas/creditCardRefund.md#creditcardrefund-accountingbookdetailcollection) | sublist/collection |
| [`creditCardRefund-accountingBookDetailElement`](../schemas/creditCardRefund.md#creditcardrefund-accountingbookdetailelement) | sublist/element |
| [`creditCardRefund-appliedRulesCollection`](../schemas/creditCardRefund.md#creditcardrefund-appliedrulescollection) | sublist/collection |
| [`creditCardRefund-appliedRulesElement`](../schemas/creditCardRefund.md#creditcardrefund-appliedruleselement) | sublist/element |
| [`creditCardRefund-expenseCollection`](../schemas/creditCardRefund.md#creditcardrefund-expensecollection) | sublist/collection |
| [`creditCardRefund-expenseElement`](../schemas/creditCardRefund.md#creditcardrefund-expenseelement) | sublist/element |
| [`creditCardRefund-item-inventoryDetail`](../schemas/creditCardRefund.md#creditcardrefund-item-inventorydetail) | related |
| [`creditCardRefund-item-inventoryDetail-inventoryAssignmentCollection`](../schemas/creditCardRefund.md#creditcardrefund-item-inventorydetail-inventoryassignmentcollection) | sublist/collection |
| [`creditCardRefund-item-inventoryDetail-inventoryAssignmentElement`](../schemas/creditCardRefund.md#creditcardrefund-item-inventorydetail-inventoryassignmentelement) | sublist/element |
| [`creditCardRefund-item-landedCost`](../schemas/creditCardRefund.md#creditcardrefund-item-landedcost) | related |
| [`creditCardRefund-item-landedCost-landedCostDataCollection`](../schemas/creditCardRefund.md#creditcardrefund-item-landedcost-landedcostdatacollection) | sublist/collection |
| [`creditCardRefund-item-landedCost-landedCostDataElement`](../schemas/creditCardRefund.md#creditcardrefund-item-landedcost-landedcostdataelement) | sublist/element |
| [`creditCardRefund-itemCollection`](../schemas/creditCardRefund.md#creditcardrefund-itemcollection) | sublist/collection |
| [`creditCardRefund-itemElement`](../schemas/creditCardRefund.md#creditcardrefund-itemelement) | sublist/element |
| [`creditCardRefund-landedCostsCollection`](../schemas/creditCardRefund.md#creditcardrefund-landedcostscollection) | sublist/collection |
| [`creditCardRefund-landedCostsElement`](../schemas/creditCardRefund.md#creditcardrefund-landedcostselement) | sublist/element |
| [`creditCardRefund-taxDetailsCollection`](../schemas/creditCardRefund.md#creditcardrefund-taxdetailscollection) | sublist/collection |
| [`creditCardRefund-taxDetailsElement`](../schemas/creditCardRefund.md#creditcardrefund-taxdetailselement) | sublist/element |
| [`creditCardRefundCollection`](../schemas/creditCardRefund.md#creditcardrefundcollection) | collection page |
| [`creditCardRefundSelectOptions`](../schemas/creditCardRefund.md#creditcardrefundselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`creditCardRefund-accountingBookDetailCollection`](../schemas/creditCardRefund.md#creditcardrefund-accountingbookdetailcollection) | [`creditCardRefund-accountingBookDetailElement`](../schemas/creditCardRefund.md#creditcardrefund-accountingbookdetailelement) |
| `appliedRules` | [`creditCardRefund-appliedRulesCollection`](../schemas/creditCardRefund.md#creditcardrefund-appliedrulescollection) | [`creditCardRefund-appliedRulesElement`](../schemas/creditCardRefund.md#creditcardrefund-appliedruleselement) |
| `expense` | [`creditCardRefund-expenseCollection`](../schemas/creditCardRefund.md#creditcardrefund-expensecollection) | [`creditCardRefund-expenseElement`](../schemas/creditCardRefund.md#creditcardrefund-expenseelement) |
| `item` | [`creditCardRefund-itemCollection`](../schemas/creditCardRefund.md#creditcardrefund-itemcollection) | [`creditCardRefund-itemElement`](../schemas/creditCardRefund.md#creditcardrefund-itemelement) |
| `landedCosts` | [`creditCardRefund-landedCostsCollection`](../schemas/creditCardRefund.md#creditcardrefund-landedcostscollection) | [`creditCardRefund-landedCostsElement`](../schemas/creditCardRefund.md#creditcardrefund-landedcostselement) |
| `taxDetails` | [`creditCardRefund-taxDetailsCollection`](../schemas/creditCardRefund.md#creditcardrefund-taxdetailscollection) | [`creditCardRefund-taxDetailsElement`](../schemas/creditCardRefund.md#creditcardrefund-taxdetailselement) |
