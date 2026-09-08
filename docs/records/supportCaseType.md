# supportCaseType

Browser tag `supportCaseType` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/supportCaseType`, instance `/supportCaseType/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/supportCaseType` | `operation--supportCaseType-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/supportCaseType` | `operation--supportCaseType-get` | Get list of records. |  | 200 OK → `supportCaseTypeCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/supportCaseType` | `operation--supportCaseType-patch` | Update records. | `supportCaseTypeCollection` | 202 Accepted; default → `nsError` |
| POST | `/supportCaseType` | `operation--supportCaseType-post` | Insert record. | `supportCaseType` | 200 OK → `supportCaseType`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/supportCaseType` | `operation--supportCaseType-put` | Insert or update records. | `supportCaseTypeCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/supportCaseType/{id}` | `operation--supportCaseType--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/supportCaseType/{id}` | `operation--supportCaseType--id--get` | Get record. |  | 200 OK → `supportCaseType`; 202 Accepted; default → `nsError` |
| PATCH | `/supportCaseType/{id}` | `operation--supportCaseType--id--patch` | Update record. | `supportCaseType` | 200 OK → `supportCaseType`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/supportCaseType/{id}` | `operation--supportCaseType--id--put` | Insert or update record. | `supportCaseType` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--supportCaseType-delete` | DELETE `/supportCaseType` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--supportCaseType-get` | GET `/supportCaseType` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--supportCaseType-patch` | PATCH `/supportCaseType` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--supportCaseType-post` | POST `/supportCaseType` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--supportCaseType-put` | PUT `/supportCaseType` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--supportCaseType--id--delete` | DELETE `/supportCaseType/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--supportCaseType--id--get` | GET `/supportCaseType/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--supportCaseType--id--patch` | PATCH `/supportCaseType/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--supportCaseType--id--put` | PUT `/supportCaseType/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [supportCaseType schemas](../schemas/supportCaseType.md).

| Definition | Role |
| --- | --- |
| [`supportCaseType`](../schemas/supportCaseType.md#supportcasetype) | record body |
| [`supportCaseTypeCollection`](../schemas/supportCaseType.md#supportcasetypecollection) | collection page |
| [`supportCaseTypeSelectOptions`](../schemas/supportCaseType.md#supportcasetypeselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
