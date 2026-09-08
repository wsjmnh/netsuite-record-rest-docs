# globalAccountMapping

Browser tag `globalAccountMapping` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/globalAccountMapping`, instance `/globalAccountMapping/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/globalAccountMapping` | `operation--globalAccountMapping-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/globalAccountMapping` | `operation--globalAccountMapping-get` | Get list of records. |  | 200 OK → `globalAccountMappingCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/globalAccountMapping` | `operation--globalAccountMapping-patch` | Update records. | `globalAccountMappingCollection` | 202 Accepted; default → `nsError` |
| POST | `/globalAccountMapping` | `operation--globalAccountMapping-post` | Insert record. | `globalAccountMapping` | 200 OK → `globalAccountMapping`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/globalAccountMapping` | `operation--globalAccountMapping-put` | Insert or update records. | `globalAccountMappingCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/globalAccountMapping/{id}` | `operation--globalAccountMapping--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/globalAccountMapping/{id}` | `operation--globalAccountMapping--id--get` | Get record. |  | 200 OK → `globalAccountMapping`; 202 Accepted; default → `nsError` |
| PATCH | `/globalAccountMapping/{id}` | `operation--globalAccountMapping--id--patch` | Update record. | `globalAccountMapping` | 200 OK → `globalAccountMapping`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/globalAccountMapping/{id}` | `operation--globalAccountMapping--id--put` | Insert or update record. | `globalAccountMapping` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--globalAccountMapping-delete` | DELETE `/globalAccountMapping` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--globalAccountMapping-get` | GET `/globalAccountMapping` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--globalAccountMapping-patch` | PATCH `/globalAccountMapping` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--globalAccountMapping-post` | POST `/globalAccountMapping` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--globalAccountMapping-put` | PUT `/globalAccountMapping` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--globalAccountMapping--id--delete` | DELETE `/globalAccountMapping/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--globalAccountMapping--id--get` | GET `/globalAccountMapping/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--globalAccountMapping--id--patch` | PATCH `/globalAccountMapping/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--globalAccountMapping--id--put` | PUT `/globalAccountMapping/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [globalAccountMapping schemas](../schemas/globalAccountMapping.md).

| Definition | Role |
| --- | --- |
| [`globalAccountMapping`](../schemas/globalAccountMapping.md#globalaccountmapping) | record body |
| [`globalAccountMappingCollection`](../schemas/globalAccountMapping.md#globalaccountmappingcollection) | collection page |
| [`globalAccountMappingSelectOptions`](../schemas/globalAccountMapping.md#globalaccountmappingselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
