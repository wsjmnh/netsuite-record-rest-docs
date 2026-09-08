# revRecFieldMapping

Browser tag `revRecFieldMapping` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/revRecFieldMapping`, instance `/revRecFieldMapping/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/revRecFieldMapping` | `operation--revRecFieldMapping-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/revRecFieldMapping` | `operation--revRecFieldMapping-get` | Get list of records. |  | 200 OK → `revRecFieldMappingCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/revRecFieldMapping` | `operation--revRecFieldMapping-patch` | Update records. | `revRecFieldMappingCollection` | 202 Accepted; default → `nsError` |
| POST | `/revRecFieldMapping` | `operation--revRecFieldMapping-post` | Insert record. | `revRecFieldMapping` | 200 OK → `revRecFieldMapping`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/revRecFieldMapping` | `operation--revRecFieldMapping-put` | Insert or update records. | `revRecFieldMappingCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/revRecFieldMapping/{id}` | `operation--revRecFieldMapping--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/revRecFieldMapping/{id}` | `operation--revRecFieldMapping--id--get` | Get record. |  | 200 OK → `revRecFieldMapping`; 202 Accepted; default → `nsError` |
| PATCH | `/revRecFieldMapping/{id}` | `operation--revRecFieldMapping--id--patch` | Update record. | `revRecFieldMapping` | 200 OK → `revRecFieldMapping`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/revRecFieldMapping/{id}` | `operation--revRecFieldMapping--id--put` | Insert or update record. | `revRecFieldMapping` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--revRecFieldMapping-delete` | DELETE `/revRecFieldMapping` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--revRecFieldMapping-get` | GET `/revRecFieldMapping` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--revRecFieldMapping-patch` | PATCH `/revRecFieldMapping` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--revRecFieldMapping-post` | POST `/revRecFieldMapping` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--revRecFieldMapping-put` | PUT `/revRecFieldMapping` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--revRecFieldMapping--id--delete` | DELETE `/revRecFieldMapping/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--revRecFieldMapping--id--get` | GET `/revRecFieldMapping/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--revRecFieldMapping--id--patch` | PATCH `/revRecFieldMapping/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--revRecFieldMapping--id--put` | PUT `/revRecFieldMapping/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [revRecFieldMapping schemas](../schemas/revRecFieldMapping.md).

| Definition | Role |
| --- | --- |
| [`revRecFieldMapping`](../schemas/revRecFieldMapping.md#revrecfieldmapping) | record body |
| [`revRecFieldMappingCollection`](../schemas/revRecFieldMapping.md#revrecfieldmappingcollection) | collection page |
| [`revRecFieldMappingSelectOptions`](../schemas/revRecFieldMapping.md#revrecfieldmappingselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
