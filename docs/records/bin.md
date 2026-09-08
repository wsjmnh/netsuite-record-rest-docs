# bin

Browser tag `bin` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/bin`, instance `/bin/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/bin` | `operation--bin-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/bin` | `operation--bin-get` | Get list of records. |  | 200 OK → `binCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/bin` | `operation--bin-patch` | Update records. | `binCollection` | 202 Accepted; default → `nsError` |
| POST | `/bin` | `operation--bin-post` | Insert record. | `bin` | 200 OK → `bin`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/bin` | `operation--bin-put` | Insert or update records. | `binCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/bin/{id}` | `operation--bin--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/bin/{id}` | `operation--bin--id--get` | Get record. |  | 200 OK → `bin`; 202 Accepted; default → `nsError` |
| PATCH | `/bin/{id}` | `operation--bin--id--patch` | Update record. | `bin` | 200 OK → `bin`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/bin/{id}` | `operation--bin--id--put` | Insert or update record. | `bin` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--bin-delete` | DELETE `/bin` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--bin-get` | GET `/bin` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--bin-patch` | PATCH `/bin` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--bin-post` | POST `/bin` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--bin-put` | PUT `/bin` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--bin--id--delete` | DELETE `/bin/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--bin--id--get` | GET `/bin/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--bin--id--patch` | PATCH `/bin/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--bin--id--put` | PUT `/bin/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [bin schemas](../schemas/bin.md).

| Definition | Role |
| --- | --- |
| [`bin`](../schemas/bin.md#bin) | record body |
| [`bin-inventoryBalanceCollection`](../schemas/bin.md#bin-inventorybalancecollection) | sublist/collection |
| [`bin-inventoryBalanceElement`](../schemas/bin.md#bin-inventorybalanceelement) | sublist/element |
| [`binCollection`](../schemas/bin.md#bincollection) | collection page |
| [`binSelectOptions`](../schemas/bin.md#binselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `inventoryBalance` | [`bin-inventoryBalanceCollection`](../schemas/bin.md#bin-inventorybalancecollection) | [`bin-inventoryBalanceElement`](../schemas/bin.md#bin-inventorybalanceelement) |
