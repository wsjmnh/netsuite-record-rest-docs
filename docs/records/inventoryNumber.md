# inventoryNumber

Browser tag `inventoryNumber` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/inventoryNumber`, instance `/inventoryNumber/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/inventoryNumber` | `operation--inventoryNumber-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/inventoryNumber` | `operation--inventoryNumber-get` | Get list of records. |  | 200 OK → `inventoryNumberCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/inventoryNumber` | `operation--inventoryNumber-patch` | Update records. | `inventoryNumberCollection` | 202 Accepted; default → `nsError` |
| POST | `/inventoryNumber` | `operation--inventoryNumber-post` | Insert record. | `inventoryNumber` | 200 OK → `inventoryNumber`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/inventoryNumber` | `operation--inventoryNumber-put` | Insert or update records. | `inventoryNumberCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/inventoryNumber/{id}` | `operation--inventoryNumber--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/inventoryNumber/{id}` | `operation--inventoryNumber--id--get` | Get record. |  | 200 OK → `inventoryNumber`; 202 Accepted; default → `nsError` |
| PATCH | `/inventoryNumber/{id}` | `operation--inventoryNumber--id--patch` | Update record. | `inventoryNumber` | 200 OK → `inventoryNumber`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/inventoryNumber/{id}` | `operation--inventoryNumber--id--put` | Insert or update record. | `inventoryNumber` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--inventoryNumber-delete` | DELETE `/inventoryNumber` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryNumber-get` | GET `/inventoryNumber` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryNumber-patch` | PATCH `/inventoryNumber` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryNumber-post` | POST `/inventoryNumber` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--inventoryNumber-put` | PUT `/inventoryNumber` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryNumber--id--delete` | DELETE `/inventoryNumber/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryNumber--id--get` | GET `/inventoryNumber/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryNumber--id--patch` | PATCH `/inventoryNumber/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--inventoryNumber--id--put` | PUT `/inventoryNumber/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [inventoryNumber schemas](../schemas/inventoryNumber.md).

| Definition | Role |
| --- | --- |
| [`inventoryNumber`](../schemas/inventoryNumber.md#inventorynumber) | record body |
| [`inventoryNumber-inventoryBalanceCollection`](../schemas/inventoryNumber.md#inventorynumber-inventorybalancecollection) | sublist/collection |
| [`inventoryNumber-inventoryBalanceElement`](../schemas/inventoryNumber.md#inventorynumber-inventorybalanceelement) | sublist/element |
| [`inventoryNumber-locationsCollection`](../schemas/inventoryNumber.md#inventorynumber-locationscollection) | sublist/collection |
| [`inventoryNumber-locationsElement`](../schemas/inventoryNumber.md#inventorynumber-locationselement) | sublist/element |
| [`inventoryNumberCollection`](../schemas/inventoryNumber.md#inventorynumbercollection) | collection page |
| [`inventoryNumberSelectOptions`](../schemas/inventoryNumber.md#inventorynumberselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `inventoryBalance` | [`inventoryNumber-inventoryBalanceCollection`](../schemas/inventoryNumber.md#inventorynumber-inventorybalancecollection) | [`inventoryNumber-inventoryBalanceElement`](../schemas/inventoryNumber.md#inventorynumber-inventorybalanceelement) |
| `locations` | [`inventoryNumber-locationsCollection`](../schemas/inventoryNumber.md#inventorynumber-locationscollection) | [`inventoryNumber-locationsElement`](../schemas/inventoryNumber.md#inventorynumber-locationselement) |
