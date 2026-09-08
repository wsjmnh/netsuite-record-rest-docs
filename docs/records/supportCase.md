# supportCase

Browser tag `supportCase` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/supportCase`, instance `/supportCase/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/supportCase` | `operation--supportCase-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/supportCase` | `operation--supportCase-get` | Get list of records. |  | 200 OK → `supportCaseCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/supportCase` | `operation--supportCase-patch` | Update records. | `supportCaseCollection` | 202 Accepted; default → `nsError` |
| POST | `/supportCase` | `operation--supportCase-post` | Insert record. | `supportCase` | 200 OK → `supportCase`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/supportCase` | `operation--supportCase-put` | Insert or update records. | `supportCaseCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/supportCase/{id}` | `operation--supportCase--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/supportCase/{id}` | `operation--supportCase--id--get` | Get record. |  | 200 OK → `supportCase`; 202 Accepted; default → `nsError` |
| PATCH | `/supportCase/{id}` | `operation--supportCase--id--patch` | Update record. | `supportCase` | 200 OK → `supportCase`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/supportCase/{id}` | `operation--supportCase--id--put` | Insert or update record. | `supportCase` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--supportCase-delete` | DELETE `/supportCase` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--supportCase-get` | GET `/supportCase` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--supportCase-patch` | PATCH `/supportCase` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--supportCase-post` | POST `/supportCase` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--supportCase-put` | PUT `/supportCase` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--supportCase--id--delete` | DELETE `/supportCase/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--supportCase--id--get` | GET `/supportCase/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--supportCase--id--patch` | PATCH `/supportCase/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--supportCase--id--put` | PUT `/supportCase/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [supportCase schemas](../schemas/supportCase.md).

| Definition | Role |
| --- | --- |
| [`supportCase`](../schemas/supportCase.md#supportcase) | record body |
| [`supportCase-escalateHistCollection`](../schemas/supportCase.md#supportcase-escalatehistcollection) | sublist/collection |
| [`supportCase-escalateHistElement`](../schemas/supportCase.md#supportcase-escalatehistelement) | sublist/element |
| [`supportCase-statusHistoryCollection`](../schemas/supportCase.md#supportcase-statushistorycollection) | sublist/collection |
| [`supportCase-statusHistoryElement`](../schemas/supportCase.md#supportcase-statushistoryelement) | sublist/element |
| [`supportCase-timeItemCollection`](../schemas/supportCase.md#supportcase-timeitemcollection) | sublist/collection |
| [`supportCase-timeItemElement`](../schemas/supportCase.md#supportcase-timeitemelement) | sublist/element |
| [`supportCaseCollection`](../schemas/supportCase.md#supportcasecollection) | collection page |
| [`supportCaseSelectOptions`](../schemas/supportCase.md#supportcaseselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `escalateHist` | [`supportCase-escalateHistCollection`](../schemas/supportCase.md#supportcase-escalatehistcollection) | [`supportCase-escalateHistElement`](../schemas/supportCase.md#supportcase-escalatehistelement) |
| `statusHistory` | [`supportCase-statusHistoryCollection`](../schemas/supportCase.md#supportcase-statushistorycollection) | [`supportCase-statusHistoryElement`](../schemas/supportCase.md#supportcase-statushistoryelement) |
| `timeItem` | [`supportCase-timeItemCollection`](../schemas/supportCase.md#supportcase-timeitemcollection) | [`supportCase-timeItemElement`](../schemas/supportCase.md#supportcase-timeitemelement) |
