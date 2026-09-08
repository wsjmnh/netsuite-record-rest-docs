# creditCardCharge

Browser tag `creditCardCharge` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/creditCardCharge`, instance `/creditCardCharge/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/creditCardCharge` | `operation--creditCardCharge-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/creditCardCharge` | `operation--creditCardCharge-get` | Get list of records. |  | 200 OK → `creditCardChargeCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/creditCardCharge` | `operation--creditCardCharge-patch` | Update records. | `creditCardChargeCollection` | 202 Accepted; default → `nsError` |
| POST | `/creditCardCharge` | `operation--creditCardCharge-post` | Insert record. | `creditCardCharge` | 200 OK → `creditCardCharge`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/creditCardCharge` | `operation--creditCardCharge-put` | Insert or update records. | `creditCardChargeCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/creditCardCharge/{id}` | `operation--creditCardCharge--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/creditCardCharge/{id}` | `operation--creditCardCharge--id--get` | Get record. |  | 200 OK → `creditCardCharge`; 202 Accepted; default → `nsError` |
| PATCH | `/creditCardCharge/{id}` | `operation--creditCardCharge--id--patch` | Update record. | `creditCardCharge` | 200 OK → `creditCardCharge`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/creditCardCharge/{id}` | `operation--creditCardCharge--id--put` | Insert or update record. | `creditCardCharge` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--creditCardCharge-delete` | DELETE `/creditCardCharge` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--creditCardCharge-get` | GET `/creditCardCharge` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--creditCardCharge-patch` | PATCH `/creditCardCharge` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--creditCardCharge-post` | POST `/creditCardCharge` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--creditCardCharge-put` | PUT `/creditCardCharge` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--creditCardCharge--id--delete` | DELETE `/creditCardCharge/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--creditCardCharge--id--get` | GET `/creditCardCharge/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--creditCardCharge--id--patch` | PATCH `/creditCardCharge/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--creditCardCharge--id--put` | PUT `/creditCardCharge/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [creditCardCharge schemas](../schemas/creditCardCharge.md).

| Definition | Role |
| --- | --- |
| [`creditCardCharge`](../schemas/creditCardCharge.md#creditcardcharge) | record body |
| [`creditCardCharge-accountingBookDetailCollection`](../schemas/creditCardCharge.md#creditcardcharge-accountingbookdetailcollection) | sublist/collection |
| [`creditCardCharge-accountingBookDetailElement`](../schemas/creditCardCharge.md#creditcardcharge-accountingbookdetailelement) | sublist/element |
| [`creditCardCharge-appliedRulesCollection`](../schemas/creditCardCharge.md#creditcardcharge-appliedrulescollection) | sublist/collection |
| [`creditCardCharge-appliedRulesElement`](../schemas/creditCardCharge.md#creditcardcharge-appliedruleselement) | sublist/element |
| [`creditCardCharge-expenseCollection`](../schemas/creditCardCharge.md#creditcardcharge-expensecollection) | sublist/collection |
| [`creditCardCharge-expenseElement`](../schemas/creditCardCharge.md#creditcardcharge-expenseelement) | sublist/element |
| [`creditCardCharge-item-inventoryDetail`](../schemas/creditCardCharge.md#creditcardcharge-item-inventorydetail) | related |
| [`creditCardCharge-item-inventoryDetail-inventoryAssignmentCollection`](../schemas/creditCardCharge.md#creditcardcharge-item-inventorydetail-inventoryassignmentcollection) | sublist/collection |
| [`creditCardCharge-item-inventoryDetail-inventoryAssignmentElement`](../schemas/creditCardCharge.md#creditcardcharge-item-inventorydetail-inventoryassignmentelement) | sublist/element |
| [`creditCardCharge-item-landedCost`](../schemas/creditCardCharge.md#creditcardcharge-item-landedcost) | related |
| [`creditCardCharge-item-landedCost-landedCostDataCollection`](../schemas/creditCardCharge.md#creditcardcharge-item-landedcost-landedcostdatacollection) | sublist/collection |
| [`creditCardCharge-item-landedCost-landedCostDataElement`](../schemas/creditCardCharge.md#creditcardcharge-item-landedcost-landedcostdataelement) | sublist/element |
| [`creditCardCharge-itemCollection`](../schemas/creditCardCharge.md#creditcardcharge-itemcollection) | sublist/collection |
| [`creditCardCharge-itemElement`](../schemas/creditCardCharge.md#creditcardcharge-itemelement) | sublist/element |
| [`creditCardCharge-landedCostsCollection`](../schemas/creditCardCharge.md#creditcardcharge-landedcostscollection) | sublist/collection |
| [`creditCardCharge-landedCostsElement`](../schemas/creditCardCharge.md#creditcardcharge-landedcostselement) | sublist/element |
| [`creditCardCharge-taxDetailsCollection`](../schemas/creditCardCharge.md#creditcardcharge-taxdetailscollection) | sublist/collection |
| [`creditCardCharge-taxDetailsElement`](../schemas/creditCardCharge.md#creditcardcharge-taxdetailselement) | sublist/element |
| [`creditCardChargeCollection`](../schemas/creditCardCharge.md#creditcardchargecollection) | collection page |
| [`creditCardChargeSelectOptions`](../schemas/creditCardCharge.md#creditcardchargeselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`creditCardCharge-accountingBookDetailCollection`](../schemas/creditCardCharge.md#creditcardcharge-accountingbookdetailcollection) | [`creditCardCharge-accountingBookDetailElement`](../schemas/creditCardCharge.md#creditcardcharge-accountingbookdetailelement) |
| `appliedRules` | [`creditCardCharge-appliedRulesCollection`](../schemas/creditCardCharge.md#creditcardcharge-appliedrulescollection) | [`creditCardCharge-appliedRulesElement`](../schemas/creditCardCharge.md#creditcardcharge-appliedruleselement) |
| `expense` | [`creditCardCharge-expenseCollection`](../schemas/creditCardCharge.md#creditcardcharge-expensecollection) | [`creditCardCharge-expenseElement`](../schemas/creditCardCharge.md#creditcardcharge-expenseelement) |
| `item` | [`creditCardCharge-itemCollection`](../schemas/creditCardCharge.md#creditcardcharge-itemcollection) | [`creditCardCharge-itemElement`](../schemas/creditCardCharge.md#creditcardcharge-itemelement) |
| `landedCosts` | [`creditCardCharge-landedCostsCollection`](../schemas/creditCardCharge.md#creditcardcharge-landedcostscollection) | [`creditCardCharge-landedCostsElement`](../schemas/creditCardCharge.md#creditcardcharge-landedcostselement) |
| `taxDetails` | [`creditCardCharge-taxDetailsCollection`](../schemas/creditCardCharge.md#creditcardcharge-taxdetailscollection) | [`creditCardCharge-taxDetailsElement`](../schemas/creditCardCharge.md#creditcardcharge-taxdetailselement) |
