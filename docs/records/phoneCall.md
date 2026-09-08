# phoneCall

Browser tag `phoneCall` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/phoneCall`, instance `/phoneCall/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/phoneCall` | `operation--phoneCall-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/phoneCall` | `operation--phoneCall-get` | Get list of records. |  | 200 OK → `phoneCallCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/phoneCall` | `operation--phoneCall-patch` | Update records. | `phoneCallCollection` | 202 Accepted; default → `nsError` |
| POST | `/phoneCall` | `operation--phoneCall-post` | Insert record. | `phoneCall` | 200 OK → `phoneCall`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/phoneCall` | `operation--phoneCall-put` | Insert or update records. | `phoneCallCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/phoneCall/{id}` | `operation--phoneCall--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/phoneCall/{id}` | `operation--phoneCall--id--get` | Get record. |  | 200 OK → `phoneCall`; 202 Accepted; default → `nsError` |
| PATCH | `/phoneCall/{id}` | `operation--phoneCall--id--patch` | Update record. | `phoneCall` | 200 OK → `phoneCall`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/phoneCall/{id}` | `operation--phoneCall--id--put` | Insert or update record. | `phoneCall` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--phoneCall-delete` | DELETE `/phoneCall` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--phoneCall-get` | GET `/phoneCall` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--phoneCall-patch` | PATCH `/phoneCall` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--phoneCall-post` | POST `/phoneCall` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--phoneCall-put` | PUT `/phoneCall` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--phoneCall--id--delete` | DELETE `/phoneCall/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--phoneCall--id--get` | GET `/phoneCall/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--phoneCall--id--patch` | PATCH `/phoneCall/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--phoneCall--id--put` | PUT `/phoneCall/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [phoneCall schemas](../schemas/phoneCall.md).

| Definition | Role |
| --- | --- |
| [`phoneCall`](../schemas/phoneCall.md#phonecall) | record body |
| [`phoneCall-timeItemCollection`](../schemas/phoneCall.md#phonecall-timeitemcollection) | sublist/collection |
| [`phoneCall-timeItemElement`](../schemas/phoneCall.md#phonecall-timeitemelement) | sublist/element |
| [`phoneCallCollection`](../schemas/phoneCall.md#phonecallcollection) | collection page |
| [`phoneCallSelectOptions`](../schemas/phoneCall.md#phonecallselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `timeItem` | [`phoneCall-timeItemCollection`](../schemas/phoneCall.md#phonecall-timeitemcollection) | [`phoneCall-timeItemElement`](../schemas/phoneCall.md#phonecall-timeitemelement) |
