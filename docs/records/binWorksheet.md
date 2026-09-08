# binWorksheet

Browser tag `binWorksheet` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/binWorksheet`, instance `/binWorksheet/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/binWorksheet` | `operation--binWorksheet-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/binWorksheet` | `operation--binWorksheet-get` | Get list of records. |  | 200 OK → `binWorksheetCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/binWorksheet` | `operation--binWorksheet-patch` | Update records. | `binWorksheetCollection` | 202 Accepted; default → `nsError` |
| POST | `/binWorksheet` | `operation--binWorksheet-post` | Insert record. | `binWorksheet` | 200 OK → `binWorksheet`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/binWorksheet` | `operation--binWorksheet-put` | Insert or update records. | `binWorksheetCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/binWorksheet/{id}` | `operation--binWorksheet--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/binWorksheet/{id}` | `operation--binWorksheet--id--get` | Get record. |  | 200 OK → `binWorksheet`; 202 Accepted; default → `nsError` |
| PATCH | `/binWorksheet/{id}` | `operation--binWorksheet--id--patch` | Update record. | `binWorksheet` | 200 OK → `binWorksheet`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/binWorksheet/{id}` | `operation--binWorksheet--id--put` | Insert or update record. | `binWorksheet` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--binWorksheet-delete` | DELETE `/binWorksheet` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--binWorksheet-get` | GET `/binWorksheet` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--binWorksheet-patch` | PATCH `/binWorksheet` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--binWorksheet-post` | POST `/binWorksheet` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--binWorksheet-put` | PUT `/binWorksheet` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--binWorksheet--id--delete` | DELETE `/binWorksheet/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--binWorksheet--id--get` | GET `/binWorksheet/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--binWorksheet--id--patch` | PATCH `/binWorksheet/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--binWorksheet--id--put` | PUT `/binWorksheet/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [binWorksheet schemas](../schemas/binWorksheet.md).

| Definition | Role |
| --- | --- |
| [`binWorksheet`](../schemas/binWorksheet.md#binworksheet) | record body |
| [`binWorksheet-item-inventoryDetail`](../schemas/binWorksheet.md#binworksheet-item-inventorydetail) | related |
| [`binWorksheet-item-inventoryDetail-inventoryAssignmentCollection`](../schemas/binWorksheet.md#binworksheet-item-inventorydetail-inventoryassignmentcollection) | sublist/collection |
| [`binWorksheet-item-inventoryDetail-inventoryAssignmentElement`](../schemas/binWorksheet.md#binworksheet-item-inventorydetail-inventoryassignmentelement) | sublist/element |
| [`binWorksheet-itemCollection`](../schemas/binWorksheet.md#binworksheet-itemcollection) | sublist/collection |
| [`binWorksheet-itemElement`](../schemas/binWorksheet.md#binworksheet-itemelement) | sublist/element |
| [`binWorksheetCollection`](../schemas/binWorksheet.md#binworksheetcollection) | collection page |
| [`binWorksheetSelectOptions`](../schemas/binWorksheet.md#binworksheetselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `item` | [`binWorksheet-itemCollection`](../schemas/binWorksheet.md#binworksheet-itemcollection) | [`binWorksheet-itemElement`](../schemas/binWorksheet.md#binworksheet-itemelement) |
