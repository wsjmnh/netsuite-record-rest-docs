# inventoryStatus

Browser tag `inventoryStatus` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/inventoryStatus`, instance `/inventoryStatus/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/inventoryStatus` | `operation--inventoryStatus-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/inventoryStatus` | `operation--inventoryStatus-get` | Get list of records. |  | 200 OK → `inventoryStatusCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/inventoryStatus` | `operation--inventoryStatus-patch` | Update records. | `inventoryStatusCollection` | 202 Accepted; default → `nsError` |
| POST | `/inventoryStatus` | `operation--inventoryStatus-post` | Insert record. | `inventoryStatus` | 200 OK → `inventoryStatus`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/inventoryStatus` | `operation--inventoryStatus-put` | Insert or update records. | `inventoryStatusCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/inventoryStatus/{id}` | `operation--inventoryStatus--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/inventoryStatus/{id}` | `operation--inventoryStatus--id--get` | Get record. |  | 200 OK → `inventoryStatus`; 202 Accepted; default → `nsError` |
| PATCH | `/inventoryStatus/{id}` | `operation--inventoryStatus--id--patch` | Update record. | `inventoryStatus` | 200 OK → `inventoryStatus`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/inventoryStatus/{id}` | `operation--inventoryStatus--id--put` | Insert or update record. | `inventoryStatus` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--inventoryStatus-delete` | DELETE `/inventoryStatus` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryStatus-get` | GET `/inventoryStatus` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryStatus-patch` | PATCH `/inventoryStatus` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryStatus-post` | POST `/inventoryStatus` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--inventoryStatus-put` | PUT `/inventoryStatus` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryStatus--id--delete` | DELETE `/inventoryStatus/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryStatus--id--get` | GET `/inventoryStatus/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryStatus--id--patch` | PATCH `/inventoryStatus/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--inventoryStatus--id--put` | PUT `/inventoryStatus/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [inventoryStatus schemas](../schemas/inventoryStatus.md).

| Definition | Role |
| --- | --- |
| [`inventoryStatus`](../schemas/inventoryStatus.md#inventorystatus) | record body |
| [`inventoryStatus-inventoryBalanceCollection`](../schemas/inventoryStatus.md#inventorystatus-inventorybalancecollection) | sublist/collection |
| [`inventoryStatus-inventoryBalanceElement`](../schemas/inventoryStatus.md#inventorystatus-inventorybalanceelement) | sublist/element |
| [`inventoryStatus-translationsCollection`](../schemas/inventoryStatus.md#inventorystatus-translationscollection) | sublist/collection |
| [`inventoryStatus-translationsElement`](../schemas/inventoryStatus.md#inventorystatus-translationselement) | sublist/element |
| [`inventoryStatusCollection`](../schemas/inventoryStatus.md#inventorystatuscollection) | collection page |
| [`inventoryStatusSelectOptions`](../schemas/inventoryStatus.md#inventorystatusselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `inventoryBalance` | [`inventoryStatus-inventoryBalanceCollection`](../schemas/inventoryStatus.md#inventorystatus-inventorybalancecollection) | [`inventoryStatus-inventoryBalanceElement`](../schemas/inventoryStatus.md#inventorystatus-inventorybalanceelement) |
| `translations` | [`inventoryStatus-translationsCollection`](../schemas/inventoryStatus.md#inventorystatus-translationscollection) | [`inventoryStatus-translationsElement`](../schemas/inventoryStatus.md#inventorystatus-translationselement) |
