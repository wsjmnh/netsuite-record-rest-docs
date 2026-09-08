# fulfillmentRequest

Browser tag `fulfillmentRequest` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/fulfillmentRequest`, instance `/fulfillmentRequest/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/fulfillmentRequest` | `operation--fulfillmentRequest-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/fulfillmentRequest` | `operation--fulfillmentRequest-get` | Get list of records. |  | 200 OK → `fulfillmentRequestCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/fulfillmentRequest` | `operation--fulfillmentRequest-patch` | Update records. | `fulfillmentRequestCollection` | 202 Accepted; default → `nsError` |
| POST | `/fulfillmentRequest` | `operation--fulfillmentRequest-post` | Insert record. | `fulfillmentRequest` | 200 OK → `fulfillmentRequest`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/fulfillmentRequest` | `operation--fulfillmentRequest-put` | Insert or update records. | `fulfillmentRequestCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/fulfillmentRequest/{id}` | `operation--fulfillmentRequest--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/fulfillmentRequest/{id}` | `operation--fulfillmentRequest--id--get` | Get record. |  | 200 OK → `fulfillmentRequest`; 202 Accepted; default → `nsError` |
| PATCH | `/fulfillmentRequest/{id}` | `operation--fulfillmentRequest--id--patch` | Update record. | `fulfillmentRequest` | 200 OK → `fulfillmentRequest`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/fulfillmentRequest/{id}` | `operation--fulfillmentRequest--id--put` | Insert or update record. | `fulfillmentRequest` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--fulfillmentRequest-delete` | DELETE `/fulfillmentRequest` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--fulfillmentRequest-get` | GET `/fulfillmentRequest` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--fulfillmentRequest-patch` | PATCH `/fulfillmentRequest` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--fulfillmentRequest-post` | POST `/fulfillmentRequest` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--fulfillmentRequest-put` | PUT `/fulfillmentRequest` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--fulfillmentRequest--id--delete` | DELETE `/fulfillmentRequest/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--fulfillmentRequest--id--get` | GET `/fulfillmentRequest/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--fulfillmentRequest--id--patch` | PATCH `/fulfillmentRequest/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--fulfillmentRequest--id--put` | PUT `/fulfillmentRequest/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [fulfillmentRequest schemas](../schemas/fulfillmentRequest.md).

| Definition | Role |
| --- | --- |
| [`fulfillmentRequest`](../schemas/fulfillmentRequest.md#fulfillmentrequest) | record body |
| [`fulfillmentRequest-fulfillmentExceptionCollection`](../schemas/fulfillmentRequest.md#fulfillmentrequest-fulfillmentexceptioncollection) | sublist/collection |
| [`fulfillmentRequest-fulfillmentExceptionElement`](../schemas/fulfillmentRequest.md#fulfillmentrequest-fulfillmentexceptionelement) | sublist/element |
| [`fulfillmentRequest-item-fulfillmentItemExceptionCollection`](../schemas/fulfillmentRequest.md#fulfillmentrequest-item-fulfillmentitemexceptioncollection) | sublist/collection |
| [`fulfillmentRequest-item-fulfillmentItemExceptionElement`](../schemas/fulfillmentRequest.md#fulfillmentrequest-item-fulfillmentitemexceptionelement) | sublist/element |
| [`fulfillmentRequest-item-inventoryDetail`](../schemas/fulfillmentRequest.md#fulfillmentrequest-item-inventorydetail) | related |
| [`fulfillmentRequest-item-inventoryDetail-inventoryAssignmentCollection`](../schemas/fulfillmentRequest.md#fulfillmentrequest-item-inventorydetail-inventoryassignmentcollection) | sublist/collection |
| [`fulfillmentRequest-item-inventoryDetail-inventoryAssignmentElement`](../schemas/fulfillmentRequest.md#fulfillmentrequest-item-inventorydetail-inventoryassignmentelement) | sublist/element |
| [`fulfillmentRequest-itemCollection`](../schemas/fulfillmentRequest.md#fulfillmentrequest-itemcollection) | sublist/collection |
| [`fulfillmentRequest-itemElement`](../schemas/fulfillmentRequest.md#fulfillmentrequest-itemelement) | sublist/element |
| [`fulfillmentRequestCollection`](../schemas/fulfillmentRequest.md#fulfillmentrequestcollection) | collection page |
| [`fulfillmentRequestSelectOptions`](../schemas/fulfillmentRequest.md#fulfillmentrequestselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `fulfillmentException` | [`fulfillmentRequest-fulfillmentExceptionCollection`](../schemas/fulfillmentRequest.md#fulfillmentrequest-fulfillmentexceptioncollection) | [`fulfillmentRequest-fulfillmentExceptionElement`](../schemas/fulfillmentRequest.md#fulfillmentrequest-fulfillmentexceptionelement) |
| `item` | [`fulfillmentRequest-itemCollection`](../schemas/fulfillmentRequest.md#fulfillmentrequest-itemcollection) | [`fulfillmentRequest-itemElement`](../schemas/fulfillmentRequest.md#fulfillmentrequest-itemelement) |
