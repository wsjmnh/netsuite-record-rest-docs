# inboundShipment

Browser tag `inboundShipment` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/inboundShipment`, instance `/inboundShipment/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/inboundShipment` | `operation--inboundShipment-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/inboundShipment` | `operation--inboundShipment-get` | Get list of records. |  | 200 OK → `inboundShipmentCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/inboundShipment` | `operation--inboundShipment-patch` | Update records. | `inboundShipmentCollection` | 202 Accepted; default → `nsError` |
| POST | `/inboundShipment` | `operation--inboundShipment-post` | Insert record. | `inboundShipment` | 200 OK → `inboundShipment`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/inboundShipment` | `operation--inboundShipment-put` | Insert or update records. | `inboundShipmentCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/inboundShipment/{id}` | `operation--inboundShipment--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/inboundShipment/{id}` | `operation--inboundShipment--id--get` | Get record. |  | 200 OK → `inboundShipment`; 202 Accepted; default → `nsError` |
| PATCH | `/inboundShipment/{id}` | `operation--inboundShipment--id--patch` | Update record. | `inboundShipment` | 200 OK → `inboundShipment`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/inboundShipment/{id}` | `operation--inboundShipment--id--put` | Insert or update record. | `inboundShipment` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--inboundShipment-delete` | DELETE `/inboundShipment` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inboundShipment-get` | GET `/inboundShipment` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inboundShipment-patch` | PATCH `/inboundShipment` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inboundShipment-post` | POST `/inboundShipment` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--inboundShipment-put` | PUT `/inboundShipment` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inboundShipment--id--delete` | DELETE `/inboundShipment/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inboundShipment--id--get` | GET `/inboundShipment/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inboundShipment--id--patch` | PATCH `/inboundShipment/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--inboundShipment--id--put` | PUT `/inboundShipment/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [inboundShipment schemas](../schemas/inboundShipment.md).

| Definition | Role |
| --- | --- |
| [`inboundShipment`](../schemas/inboundShipment.md#inboundshipment) | record body |
| [`inboundShipment-items-inventorydetail`](../schemas/inboundShipment.md#inboundshipment-items-inventorydetail) | related |
| [`inboundShipment-items-inventorydetail-inventoryAssignmentCollection`](../schemas/inboundShipment.md#inboundshipment-items-inventorydetail-inventoryassignmentcollection) | sublist/collection |
| [`inboundShipment-items-inventorydetail-inventoryAssignmentElement`](../schemas/inboundShipment.md#inboundshipment-items-inventorydetail-inventoryassignmentelement) | sublist/element |
| [`inboundShipment-itemsCollection`](../schemas/inboundShipment.md#inboundshipment-itemscollection) | sublist/collection |
| [`inboundShipment-itemsElement`](../schemas/inboundShipment.md#inboundshipment-itemselement) | sublist/element |
| [`inboundShipment-landedCostCollection`](../schemas/inboundShipment.md#inboundshipment-landedcostcollection) | sublist/collection |
| [`inboundShipment-landedCostElement`](../schemas/inboundShipment.md#inboundshipment-landedcostelement) | sublist/element |
| [`inboundShipmentCollection`](../schemas/inboundShipment.md#inboundshipmentcollection) | collection page |
| [`inboundShipmentSelectOptions`](../schemas/inboundShipment.md#inboundshipmentselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `items` | [`inboundShipment-itemsCollection`](../schemas/inboundShipment.md#inboundshipment-itemscollection) | [`inboundShipment-itemsElement`](../schemas/inboundShipment.md#inboundshipment-itemselement) |
| `landedCost` | [`inboundShipment-landedCostCollection`](../schemas/inboundShipment.md#inboundshipment-landedcostcollection) | [`inboundShipment-landedCostElement`](../schemas/inboundShipment.md#inboundshipment-landedcostelement) |
