# inventoryCostRevaluation

Browser tag `inventoryCostRevaluation` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/inventoryCostRevaluation`, instance `/inventoryCostRevaluation/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/inventoryCostRevaluation` | `operation--inventoryCostRevaluation-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/inventoryCostRevaluation` | `operation--inventoryCostRevaluation-get` | Get list of records. |  | 200 OK → `inventoryCostRevaluationCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/inventoryCostRevaluation` | `operation--inventoryCostRevaluation-patch` | Update records. | `inventoryCostRevaluationCollection` | 202 Accepted; default → `nsError` |
| POST | `/inventoryCostRevaluation` | `operation--inventoryCostRevaluation-post` | Insert record. | `inventoryCostRevaluation` | 200 OK → `inventoryCostRevaluation`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/inventoryCostRevaluation` | `operation--inventoryCostRevaluation-put` | Insert or update records. | `inventoryCostRevaluationCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/inventoryCostRevaluation/{id}` | `operation--inventoryCostRevaluation--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/inventoryCostRevaluation/{id}` | `operation--inventoryCostRevaluation--id--get` | Get record. |  | 200 OK → `inventoryCostRevaluation`; 202 Accepted; default → `nsError` |
| PATCH | `/inventoryCostRevaluation/{id}` | `operation--inventoryCostRevaluation--id--patch` | Update record. | `inventoryCostRevaluation` | 200 OK → `inventoryCostRevaluation`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/inventoryCostRevaluation/{id}` | `operation--inventoryCostRevaluation--id--put` | Insert or update record. | `inventoryCostRevaluation` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--inventoryCostRevaluation-delete` | DELETE `/inventoryCostRevaluation` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryCostRevaluation-get` | GET `/inventoryCostRevaluation` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryCostRevaluation-patch` | PATCH `/inventoryCostRevaluation` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryCostRevaluation-post` | POST `/inventoryCostRevaluation` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--inventoryCostRevaluation-put` | PUT `/inventoryCostRevaluation` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryCostRevaluation--id--delete` | DELETE `/inventoryCostRevaluation/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryCostRevaluation--id--get` | GET `/inventoryCostRevaluation/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryCostRevaluation--id--patch` | PATCH `/inventoryCostRevaluation/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--inventoryCostRevaluation--id--put` | PUT `/inventoryCostRevaluation/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [inventoryCostRevaluation schemas](../schemas/inventoryCostRevaluation.md).

| Definition | Role |
| --- | --- |
| [`inventoryCostRevaluation`](../schemas/inventoryCostRevaluation.md#inventorycostrevaluation) | record body |
| [`inventoryCostRevaluation-accountingBookDetailCollection`](../schemas/inventoryCostRevaluation.md#inventorycostrevaluation-accountingbookdetailcollection) | sublist/collection |
| [`inventoryCostRevaluation-accountingBookDetailElement`](../schemas/inventoryCostRevaluation.md#inventorycostrevaluation-accountingbookdetailelement) | sublist/element |
| [`inventoryCostRevaluation-costComponentCollection`](../schemas/inventoryCostRevaluation.md#inventorycostrevaluation-costcomponentcollection) | sublist/collection |
| [`inventoryCostRevaluation-costComponentElement`](../schemas/inventoryCostRevaluation.md#inventorycostrevaluation-costcomponentelement) | sublist/element |
| [`inventoryCostRevaluationCollection`](../schemas/inventoryCostRevaluation.md#inventorycostrevaluationcollection) | collection page |
| [`inventoryCostRevaluationSelectOptions`](../schemas/inventoryCostRevaluation.md#inventorycostrevaluationselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`inventoryCostRevaluation-accountingBookDetailCollection`](../schemas/inventoryCostRevaluation.md#inventorycostrevaluation-accountingbookdetailcollection) | [`inventoryCostRevaluation-accountingBookDetailElement`](../schemas/inventoryCostRevaluation.md#inventorycostrevaluation-accountingbookdetailelement) |
| `costComponent` | [`inventoryCostRevaluation-costComponentCollection`](../schemas/inventoryCostRevaluation.md#inventorycostrevaluation-costcomponentcollection) | [`inventoryCostRevaluation-costComponentElement`](../schemas/inventoryCostRevaluation.md#inventorycostrevaluation-costcomponentelement) |
