# inventoryTransfer

Browser tag `inventoryTransfer` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/inventoryTransfer`, instance `/inventoryTransfer/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/inventoryTransfer` | `operation--inventoryTransfer-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/inventoryTransfer` | `operation--inventoryTransfer-get` | Get list of records. |  | 200 OK → `inventoryTransferCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/inventoryTransfer` | `operation--inventoryTransfer-patch` | Update records. | `inventoryTransferCollection` | 202 Accepted; default → `nsError` |
| POST | `/inventoryTransfer` | `operation--inventoryTransfer-post` | Insert record. | `inventoryTransfer` | 200 OK → `inventoryTransfer`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/inventoryTransfer` | `operation--inventoryTransfer-put` | Insert or update records. | `inventoryTransferCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/inventoryTransfer/{id}` | `operation--inventoryTransfer--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/inventoryTransfer/{id}` | `operation--inventoryTransfer--id--get` | Get record. |  | 200 OK → `inventoryTransfer`; 202 Accepted; default → `nsError` |
| PATCH | `/inventoryTransfer/{id}` | `operation--inventoryTransfer--id--patch` | Update record. | `inventoryTransfer` | 200 OK → `inventoryTransfer`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/inventoryTransfer/{id}` | `operation--inventoryTransfer--id--put` | Insert or update record. | `inventoryTransfer` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--inventoryTransfer-delete` | DELETE `/inventoryTransfer` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryTransfer-get` | GET `/inventoryTransfer` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryTransfer-patch` | PATCH `/inventoryTransfer` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryTransfer-post` | POST `/inventoryTransfer` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--inventoryTransfer-put` | PUT `/inventoryTransfer` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryTransfer--id--delete` | DELETE `/inventoryTransfer/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryTransfer--id--get` | GET `/inventoryTransfer/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryTransfer--id--patch` | PATCH `/inventoryTransfer/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--inventoryTransfer--id--put` | PUT `/inventoryTransfer/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [inventoryTransfer schemas](../schemas/inventoryTransfer.md).

| Definition | Role |
| --- | --- |
| [`inventoryTransfer`](../schemas/inventoryTransfer.md#inventorytransfer) | record body |
| [`inventoryTransfer-inventory-inventoryDetail`](../schemas/inventoryTransfer.md#inventorytransfer-inventory-inventorydetail) | related |
| [`inventoryTransfer-inventory-inventoryDetail-inventoryAssignmentCollection`](../schemas/inventoryTransfer.md#inventorytransfer-inventory-inventorydetail-inventoryassignmentcollection) | sublist/collection |
| [`inventoryTransfer-inventory-inventoryDetail-inventoryAssignmentElement`](../schemas/inventoryTransfer.md#inventorytransfer-inventory-inventorydetail-inventoryassignmentelement) | sublist/element |
| [`inventoryTransfer-inventoryCollection`](../schemas/inventoryTransfer.md#inventorytransfer-inventorycollection) | sublist/collection |
| [`inventoryTransfer-inventoryElement`](../schemas/inventoryTransfer.md#inventorytransfer-inventoryelement) | sublist/element |
| [`inventoryTransferCollection`](../schemas/inventoryTransfer.md#inventorytransfercollection) | collection page |
| [`inventoryTransferSelectOptions`](../schemas/inventoryTransfer.md#inventorytransferselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `inventory` | [`inventoryTransfer-inventoryCollection`](../schemas/inventoryTransfer.md#inventorytransfer-inventorycollection) | [`inventoryTransfer-inventoryElement`](../schemas/inventoryTransfer.md#inventorytransfer-inventoryelement) |
