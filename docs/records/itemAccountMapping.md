# itemAccountMapping

Browser tag `itemAccountMapping` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/itemAccountMapping`, instance `/itemAccountMapping/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/itemAccountMapping` | `operation--itemAccountMapping-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/itemAccountMapping` | `operation--itemAccountMapping-get` | Get list of records. |  | 200 OK → `itemAccountMappingCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/itemAccountMapping` | `operation--itemAccountMapping-patch` | Update records. | `itemAccountMappingCollection` | 202 Accepted; default → `nsError` |
| POST | `/itemAccountMapping` | `operation--itemAccountMapping-post` | Insert record. | `itemAccountMapping` | 200 OK → `itemAccountMapping`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/itemAccountMapping` | `operation--itemAccountMapping-put` | Insert or update records. | `itemAccountMappingCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/itemAccountMapping/{id}` | `operation--itemAccountMapping--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/itemAccountMapping/{id}` | `operation--itemAccountMapping--id--get` | Get record. |  | 200 OK → `itemAccountMapping`; 202 Accepted; default → `nsError` |
| PATCH | `/itemAccountMapping/{id}` | `operation--itemAccountMapping--id--patch` | Update record. | `itemAccountMapping` | 200 OK → `itemAccountMapping`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/itemAccountMapping/{id}` | `operation--itemAccountMapping--id--put` | Insert or update record. | `itemAccountMapping` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--itemAccountMapping-delete` | DELETE `/itemAccountMapping` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemAccountMapping-get` | GET `/itemAccountMapping` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemAccountMapping-patch` | PATCH `/itemAccountMapping` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemAccountMapping-post` | POST `/itemAccountMapping` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--itemAccountMapping-put` | PUT `/itemAccountMapping` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemAccountMapping--id--delete` | DELETE `/itemAccountMapping/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemAccountMapping--id--get` | GET `/itemAccountMapping/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemAccountMapping--id--patch` | PATCH `/itemAccountMapping/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--itemAccountMapping--id--put` | PUT `/itemAccountMapping/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [itemAccountMapping schemas](../schemas/itemAccountMapping.md).

| Definition | Role |
| --- | --- |
| [`itemAccountMapping`](../schemas/itemAccountMapping.md#itemaccountmapping) | record body |
| [`itemAccountMappingCollection`](../schemas/itemAccountMapping.md#itemaccountmappingcollection) | collection page |
| [`itemAccountMappingSelectOptions`](../schemas/itemAccountMapping.md#itemaccountmappingselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
