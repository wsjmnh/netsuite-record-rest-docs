# binTransfer

Browser tag `binTransfer` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/binTransfer`, instance `/binTransfer/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/binTransfer` | `operation--binTransfer-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/binTransfer` | `operation--binTransfer-get` | Get list of records. |  | 200 OK → `binTransferCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/binTransfer` | `operation--binTransfer-patch` | Update records. | `binTransferCollection` | 202 Accepted; default → `nsError` |
| POST | `/binTransfer` | `operation--binTransfer-post` | Insert record. | `binTransfer` | 200 OK → `binTransfer`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/binTransfer` | `operation--binTransfer-put` | Insert or update records. | `binTransferCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/binTransfer/{id}` | `operation--binTransfer--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/binTransfer/{id}` | `operation--binTransfer--id--get` | Get record. |  | 200 OK → `binTransfer`; 202 Accepted; default → `nsError` |
| PATCH | `/binTransfer/{id}` | `operation--binTransfer--id--patch` | Update record. | `binTransfer` | 200 OK → `binTransfer`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/binTransfer/{id}` | `operation--binTransfer--id--put` | Insert or update record. | `binTransfer` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--binTransfer-delete` | DELETE `/binTransfer` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--binTransfer-get` | GET `/binTransfer` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--binTransfer-patch` | PATCH `/binTransfer` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--binTransfer-post` | POST `/binTransfer` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--binTransfer-put` | PUT `/binTransfer` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--binTransfer--id--delete` | DELETE `/binTransfer/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--binTransfer--id--get` | GET `/binTransfer/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--binTransfer--id--patch` | PATCH `/binTransfer/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--binTransfer--id--put` | PUT `/binTransfer/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [binTransfer schemas](../schemas/binTransfer.md).

| Definition | Role |
| --- | --- |
| [`binTransfer`](../schemas/binTransfer.md#bintransfer) | record body |
| [`binTransfer-inventory-inventoryDetail`](../schemas/binTransfer.md#bintransfer-inventory-inventorydetail) | related |
| [`binTransfer-inventory-inventoryDetail-inventoryAssignmentCollection`](../schemas/binTransfer.md#bintransfer-inventory-inventorydetail-inventoryassignmentcollection) | sublist/collection |
| [`binTransfer-inventory-inventoryDetail-inventoryAssignmentElement`](../schemas/binTransfer.md#bintransfer-inventory-inventorydetail-inventoryassignmentelement) | sublist/element |
| [`binTransfer-inventoryCollection`](../schemas/binTransfer.md#bintransfer-inventorycollection) | sublist/collection |
| [`binTransfer-inventoryElement`](../schemas/binTransfer.md#bintransfer-inventoryelement) | sublist/element |
| [`binTransferCollection`](../schemas/binTransfer.md#bintransfercollection) | collection page |
| [`binTransferSelectOptions`](../schemas/binTransfer.md#bintransferselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `inventory` | [`binTransfer-inventoryCollection`](../schemas/binTransfer.md#bintransfer-inventorycollection) | [`binTransfer-inventoryElement`](../schemas/binTransfer.md#bintransfer-inventoryelement) |
