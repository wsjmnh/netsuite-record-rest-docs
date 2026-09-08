# inventoryCount

Browser tag `inventoryCount` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/inventoryCount`, instance `/inventoryCount/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/inventoryCount` | `operation--inventoryCount-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/inventoryCount` | `operation--inventoryCount-get` | Get list of records. |  | 200 OK → `inventoryCountCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/inventoryCount` | `operation--inventoryCount-patch` | Update records. | `inventoryCountCollection` | 202 Accepted; default → `nsError` |
| POST | `/inventoryCount` | `operation--inventoryCount-post` | Insert record. | `inventoryCount` | 200 OK → `inventoryCount`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/inventoryCount` | `operation--inventoryCount-put` | Insert or update records. | `inventoryCountCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/inventoryCount/{id}` | `operation--inventoryCount--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/inventoryCount/{id}` | `operation--inventoryCount--id--get` | Get record. |  | 200 OK → `inventoryCount`; 202 Accepted; default → `nsError` |
| PATCH | `/inventoryCount/{id}` | `operation--inventoryCount--id--patch` | Update record. | `inventoryCount` | 200 OK → `inventoryCount`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/inventoryCount/{id}` | `operation--inventoryCount--id--put` | Insert or update record. | `inventoryCount` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--inventoryCount-delete` | DELETE `/inventoryCount` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryCount-get` | GET `/inventoryCount` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryCount-patch` | PATCH `/inventoryCount` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryCount-post` | POST `/inventoryCount` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--inventoryCount-put` | PUT `/inventoryCount` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryCount--id--delete` | DELETE `/inventoryCount/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryCount--id--get` | GET `/inventoryCount/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryCount--id--patch` | PATCH `/inventoryCount/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--inventoryCount--id--put` | PUT `/inventoryCount/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [inventoryCount schemas](../schemas/inventoryCount.md).

| Definition | Role |
| --- | --- |
| [`inventoryCount`](../schemas/inventoryCount.md#inventorycount) | record body |
| [`inventoryCount-item-countDetail`](../schemas/inventoryCount.md#inventorycount-item-countdetail) | related |
| [`inventoryCount-item-countDetail-inventoryDetailCollection`](../schemas/inventoryCount.md#inventorycount-item-countdetail-inventorydetailcollection) | sublist/collection |
| [`inventoryCount-item-countDetail-inventoryDetailElement`](../schemas/inventoryCount.md#inventorycount-item-countdetail-inventorydetailelement) | sublist/element |
| [`inventoryCount-itemCollection`](../schemas/inventoryCount.md#inventorycount-itemcollection) | sublist/collection |
| [`inventoryCount-itemElement`](../schemas/inventoryCount.md#inventorycount-itemelement) | sublist/element |
| [`inventoryCountCollection`](../schemas/inventoryCount.md#inventorycountcollection) | collection page |
| [`inventoryCountSelectOptions`](../schemas/inventoryCount.md#inventorycountselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `item` | [`inventoryCount-itemCollection`](../schemas/inventoryCount.md#inventorycount-itemcollection) | [`inventoryCount-itemElement`](../schemas/inventoryCount.md#inventorycount-itemelement) |
