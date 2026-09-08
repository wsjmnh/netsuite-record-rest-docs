# inventoryAdjustment

Browser tag `inventoryAdjustment` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/inventoryAdjustment`, instance `/inventoryAdjustment/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/inventoryAdjustment` | `operation--inventoryAdjustment-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/inventoryAdjustment` | `operation--inventoryAdjustment-get` | Get list of records. |  | 200 OK → `inventoryAdjustmentCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/inventoryAdjustment` | `operation--inventoryAdjustment-patch` | Update records. | `inventoryAdjustmentCollection` | 202 Accepted; default → `nsError` |
| POST | `/inventoryAdjustment` | `operation--inventoryAdjustment-post` | Insert record. | `inventoryAdjustment` | 200 OK → `inventoryAdjustment`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/inventoryAdjustment` | `operation--inventoryAdjustment-put` | Insert or update records. | `inventoryAdjustmentCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/inventoryAdjustment/{id}` | `operation--inventoryAdjustment--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/inventoryAdjustment/{id}` | `operation--inventoryAdjustment--id--get` | Get record. |  | 200 OK → `inventoryAdjustment`; 202 Accepted; default → `nsError` |
| PATCH | `/inventoryAdjustment/{id}` | `operation--inventoryAdjustment--id--patch` | Update record. | `inventoryAdjustment` | 200 OK → `inventoryAdjustment`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/inventoryAdjustment/{id}` | `operation--inventoryAdjustment--id--put` | Insert or update record. | `inventoryAdjustment` | 202 Accepted; 204 No Content; default → `nsError` |
| POST | `/inventoryAdjustment/{targetId}/!attach/contact/{attachmentId}` | `operation--inventoryAdjustment--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` | 202 Accepted; 204 No Content |
| POST | `/inventoryAdjustment/{targetId}/!detach/contact/{attachmentId}` | `operation--inventoryAdjustment--targetId---detach-contact--attachmentId--post` | Detach a contact. |  | 202 Accepted; 204 No Content |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--inventoryAdjustment-delete` | DELETE `/inventoryAdjustment` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryAdjustment-get` | GET `/inventoryAdjustment` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryAdjustment-patch` | PATCH `/inventoryAdjustment` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryAdjustment-post` | POST `/inventoryAdjustment` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--inventoryAdjustment-put` | PUT `/inventoryAdjustment` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryAdjustment--id--delete` | DELETE `/inventoryAdjustment/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryAdjustment--id--get` | GET `/inventoryAdjustment/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryAdjustment--id--patch` | PATCH `/inventoryAdjustment/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--inventoryAdjustment--id--put` | PUT `/inventoryAdjustment/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--inventoryAdjustment--targetId---attach-contact--attachmentId--post` | POST `/inventoryAdjustment/{targetId}/!attach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryAdjustment--targetId---detach-contact--attachmentId--post` | POST `/inventoryAdjustment/{targetId}/!detach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |

## Inline request bodies

### `operation--inventoryAdjustment--targetId---attach-contact--attachmentId--post`

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `role` |  | object |  |  |  |  |
| `role.externalId` |  | string |  |  |  |  |
| `role.id` |  | integer | int32 |  |  |  |


## Schema refs

Definitions owned by this record (property tables): [inventoryAdjustment schemas](../schemas/inventoryAdjustment.md).

| Definition | Role |
| --- | --- |
| [`inventoryAdjustment`](../schemas/inventoryAdjustment.md#inventoryadjustment) | record body |
| [`inventoryAdjustment-accountingBookDetailCollection`](../schemas/inventoryAdjustment.md#inventoryadjustment-accountingbookdetailcollection) | sublist/collection |
| [`inventoryAdjustment-accountingBookDetailElement`](../schemas/inventoryAdjustment.md#inventoryadjustment-accountingbookdetailelement) | sublist/element |
| [`inventoryAdjustment-inventory-inventoryDetail`](../schemas/inventoryAdjustment.md#inventoryadjustment-inventory-inventorydetail) | related |
| [`inventoryAdjustment-inventory-inventoryDetail-inventoryAssignmentCollection`](../schemas/inventoryAdjustment.md#inventoryadjustment-inventory-inventorydetail-inventoryassignmentcollection) | sublist/collection |
| [`inventoryAdjustment-inventory-inventoryDetail-inventoryAssignmentElement`](../schemas/inventoryAdjustment.md#inventoryadjustment-inventory-inventorydetail-inventoryassignmentelement) | sublist/element |
| [`inventoryAdjustment-inventoryCollection`](../schemas/inventoryAdjustment.md#inventoryadjustment-inventorycollection) | sublist/collection |
| [`inventoryAdjustment-inventoryElement`](../schemas/inventoryAdjustment.md#inventoryadjustment-inventoryelement) | sublist/element |
| [`inventoryAdjustmentCollection`](../schemas/inventoryAdjustment.md#inventoryadjustmentcollection) | collection page |
| [`inventoryAdjustmentSelectOptions`](../schemas/inventoryAdjustment.md#inventoryadjustmentselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`inventoryAdjustment-accountingBookDetailCollection`](../schemas/inventoryAdjustment.md#inventoryadjustment-accountingbookdetailcollection) | [`inventoryAdjustment-accountingBookDetailElement`](../schemas/inventoryAdjustment.md#inventoryadjustment-accountingbookdetailelement) |
| `inventory` | [`inventoryAdjustment-inventoryCollection`](../schemas/inventoryAdjustment.md#inventoryadjustment-inventorycollection) | [`inventoryAdjustment-inventoryElement`](../schemas/inventoryAdjustment.md#inventoryadjustment-inventoryelement) |

## Attach / detach

| Method | Path | Operation ID | Summary | Request body |
| --- | --- | --- | --- | --- |
| POST | `/inventoryAdjustment/{targetId}/!attach/contact/{attachmentId}` | `operation--inventoryAdjustment--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` |
| POST | `/inventoryAdjustment/{targetId}/!detach/contact/{attachmentId}` | `operation--inventoryAdjustment--targetId---detach-contact--attachmentId--post` | Detach a contact. |  |
