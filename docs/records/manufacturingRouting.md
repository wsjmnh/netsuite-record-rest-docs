# manufacturingRouting

Browser tag `manufacturingRouting` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/manufacturingRouting`, instance `/manufacturingRouting/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/manufacturingRouting` | `operation--manufacturingRouting-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/manufacturingRouting` | `operation--manufacturingRouting-get` | Get list of records. |  | 200 OK → `manufacturingRoutingCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/manufacturingRouting` | `operation--manufacturingRouting-patch` | Update records. | `manufacturingRoutingCollection` | 202 Accepted; default → `nsError` |
| POST | `/manufacturingRouting` | `operation--manufacturingRouting-post` | Insert record. | `manufacturingRouting` | 200 OK → `manufacturingRouting`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/manufacturingRouting` | `operation--manufacturingRouting-put` | Insert or update records. | `manufacturingRoutingCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/manufacturingRouting/{id}` | `operation--manufacturingRouting--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/manufacturingRouting/{id}` | `operation--manufacturingRouting--id--get` | Get record. |  | 200 OK → `manufacturingRouting`; 202 Accepted; default → `nsError` |
| PATCH | `/manufacturingRouting/{id}` | `operation--manufacturingRouting--id--patch` | Update record. | `manufacturingRouting` | 200 OK → `manufacturingRouting`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/manufacturingRouting/{id}` | `operation--manufacturingRouting--id--put` | Insert or update record. | `manufacturingRouting` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--manufacturingRouting-delete` | DELETE `/manufacturingRouting` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--manufacturingRouting-get` | GET `/manufacturingRouting` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--manufacturingRouting-patch` | PATCH `/manufacturingRouting` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--manufacturingRouting-post` | POST `/manufacturingRouting` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--manufacturingRouting-put` | PUT `/manufacturingRouting` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--manufacturingRouting--id--delete` | DELETE `/manufacturingRouting/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--manufacturingRouting--id--get` | GET `/manufacturingRouting/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--manufacturingRouting--id--patch` | PATCH `/manufacturingRouting/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--manufacturingRouting--id--put` | PUT `/manufacturingRouting/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [manufacturingRouting schemas](../schemas/manufacturingRouting.md).

| Definition | Role |
| --- | --- |
| [`manufacturingRouting`](../schemas/manufacturingRouting.md#manufacturingrouting) | record body |
| [`manufacturingRouting-routingComponentCollection`](../schemas/manufacturingRouting.md#manufacturingrouting-routingcomponentcollection) | sublist/collection |
| [`manufacturingRouting-routingComponentElement`](../schemas/manufacturingRouting.md#manufacturingrouting-routingcomponentelement) | sublist/element |
| [`manufacturingRouting-routingStepCollection`](../schemas/manufacturingRouting.md#manufacturingrouting-routingstepcollection) | sublist/collection |
| [`manufacturingRouting-routingStepElement`](../schemas/manufacturingRouting.md#manufacturingrouting-routingstepelement) | sublist/element |
| [`manufacturingRoutingCollection`](../schemas/manufacturingRouting.md#manufacturingroutingcollection) | collection page |
| [`manufacturingRoutingSelectOptions`](../schemas/manufacturingRouting.md#manufacturingroutingselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `routingComponent` | [`manufacturingRouting-routingComponentCollection`](../schemas/manufacturingRouting.md#manufacturingrouting-routingcomponentcollection) | [`manufacturingRouting-routingComponentElement`](../schemas/manufacturingRouting.md#manufacturingrouting-routingcomponentelement) |
| `routingStep` | [`manufacturingRouting-routingStepCollection`](../schemas/manufacturingRouting.md#manufacturingrouting-routingstepcollection) | [`manufacturingRouting-routingStepElement`](../schemas/manufacturingRouting.md#manufacturingrouting-routingstepelement) |
