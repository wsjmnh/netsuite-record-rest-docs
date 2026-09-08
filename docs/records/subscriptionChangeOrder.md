# subscriptionChangeOrder

Browser tag `subscriptionChangeOrder` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/subscriptionChangeOrder`, instance `/subscriptionChangeOrder/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/subscriptionChangeOrder` | `operation--subscriptionChangeOrder-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/subscriptionChangeOrder` | `operation--subscriptionChangeOrder-get` | Get list of records. |  | 200 OK → `subscriptionChangeOrderCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/subscriptionChangeOrder` | `operation--subscriptionChangeOrder-patch` | Update records. | `subscriptionChangeOrderCollection` | 202 Accepted; default → `nsError` |
| POST | `/subscriptionChangeOrder` | `operation--subscriptionChangeOrder-post` | Insert record. | `subscriptionChangeOrder` | 200 OK → `subscriptionChangeOrder`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/subscriptionChangeOrder` | `operation--subscriptionChangeOrder-put` | Insert or update records. | `subscriptionChangeOrderCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/subscriptionChangeOrder/{id}` | `operation--subscriptionChangeOrder--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/subscriptionChangeOrder/{id}` | `operation--subscriptionChangeOrder--id--get` | Get record. |  | 200 OK → `subscriptionChangeOrder`; 202 Accepted; default → `nsError` |
| PATCH | `/subscriptionChangeOrder/{id}` | `operation--subscriptionChangeOrder--id--patch` | Update record. | `subscriptionChangeOrder` | 200 OK → `subscriptionChangeOrder`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/subscriptionChangeOrder/{id}` | `operation--subscriptionChangeOrder--id--put` | Insert or update record. | `subscriptionChangeOrder` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--subscriptionChangeOrder-delete` | DELETE `/subscriptionChangeOrder` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subscriptionChangeOrder-get` | GET `/subscriptionChangeOrder` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subscriptionChangeOrder-patch` | PATCH `/subscriptionChangeOrder` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subscriptionChangeOrder-post` | POST `/subscriptionChangeOrder` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--subscriptionChangeOrder-put` | PUT `/subscriptionChangeOrder` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subscriptionChangeOrder--id--delete` | DELETE `/subscriptionChangeOrder/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subscriptionChangeOrder--id--get` | GET `/subscriptionChangeOrder/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subscriptionChangeOrder--id--patch` | PATCH `/subscriptionChangeOrder/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--subscriptionChangeOrder--id--put` | PUT `/subscriptionChangeOrder/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [subscriptionChangeOrder schemas](../schemas/subscriptionChangeOrder.md).

| Definition | Role |
| --- | --- |
| [`subscriptionChangeOrder`](../schemas/subscriptionChangeOrder.md#subscriptionchangeorder) | record body |
| [`subscriptionChangeOrder-changeOrderLineCollection`](../schemas/subscriptionChangeOrder.md#subscriptionchangeorder-changeorderlinecollection) | sublist/collection |
| [`subscriptionChangeOrder-changeOrderLineElement`](../schemas/subscriptionChangeOrder.md#subscriptionchangeorder-changeorderlineelement) | sublist/element |
| [`subscriptionChangeOrder-newSubLineCollection`](../schemas/subscriptionChangeOrder.md#subscriptionchangeorder-newsublinecollection) | sublist/collection |
| [`subscriptionChangeOrder-newSubLineElement`](../schemas/subscriptionChangeOrder.md#subscriptionchangeorder-newsublineelement) | sublist/element |
| [`subscriptionChangeOrder-renewalStepsCollection`](../schemas/subscriptionChangeOrder.md#subscriptionchangeorder-renewalstepscollection) | sublist/collection |
| [`subscriptionChangeOrder-renewalStepsElement`](../schemas/subscriptionChangeOrder.md#subscriptionchangeorder-renewalstepselement) | sublist/element |
| [`subscriptionChangeOrder-subLineCollection`](../schemas/subscriptionChangeOrder.md#subscriptionchangeorder-sublinecollection) | sublist/collection |
| [`subscriptionChangeOrder-subLineElement`](../schemas/subscriptionChangeOrder.md#subscriptionchangeorder-sublineelement) | sublist/element |
| [`subscriptionChangeOrderCollection`](../schemas/subscriptionChangeOrder.md#subscriptionchangeordercollection) | collection page |
| [`subscriptionChangeOrderSelectOptions`](../schemas/subscriptionChangeOrder.md#subscriptionchangeorderselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `changeOrderLine` | [`subscriptionChangeOrder-changeOrderLineCollection`](../schemas/subscriptionChangeOrder.md#subscriptionchangeorder-changeorderlinecollection) | [`subscriptionChangeOrder-changeOrderLineElement`](../schemas/subscriptionChangeOrder.md#subscriptionchangeorder-changeorderlineelement) |
| `newSubLine` | [`subscriptionChangeOrder-newSubLineCollection`](../schemas/subscriptionChangeOrder.md#subscriptionchangeorder-newsublinecollection) | [`subscriptionChangeOrder-newSubLineElement`](../schemas/subscriptionChangeOrder.md#subscriptionchangeorder-newsublineelement) |
| `renewalSteps` | [`subscriptionChangeOrder-renewalStepsCollection`](../schemas/subscriptionChangeOrder.md#subscriptionchangeorder-renewalstepscollection) | [`subscriptionChangeOrder-renewalStepsElement`](../schemas/subscriptionChangeOrder.md#subscriptionchangeorder-renewalstepselement) |
| `subLine` | [`subscriptionChangeOrder-subLineCollection`](../schemas/subscriptionChangeOrder.md#subscriptionchangeorder-sublinecollection) | [`subscriptionChangeOrder-subLineElement`](../schemas/subscriptionChangeOrder.md#subscriptionchangeorder-sublineelement) |
