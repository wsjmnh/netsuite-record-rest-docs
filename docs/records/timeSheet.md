# timeSheet

Browser tag `timeSheet` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/timeSheet`, instance `/timeSheet/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/timeSheet` | `operation--timeSheet-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/timeSheet` | `operation--timeSheet-get` | Get list of records. |  | 200 OK → `timeSheetCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/timeSheet` | `operation--timeSheet-patch` | Update records. | `timeSheetCollection` | 202 Accepted; default → `nsError` |
| POST | `/timeSheet` | `operation--timeSheet-post` | Insert record. | `timeSheet` | 200 OK → `timeSheet`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/timeSheet` | `operation--timeSheet-put` | Insert or update records. | `timeSheetCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/timeSheet/{id}` | `operation--timeSheet--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/timeSheet/{id}` | `operation--timeSheet--id--get` | Get record. |  | 200 OK → `timeSheet`; 202 Accepted; default → `nsError` |
| PATCH | `/timeSheet/{id}` | `operation--timeSheet--id--patch` | Update record. | `timeSheet` | 200 OK → `timeSheet`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/timeSheet/{id}` | `operation--timeSheet--id--put` | Insert or update record. | `timeSheet` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--timeSheet-delete` | DELETE `/timeSheet` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--timeSheet-get` | GET `/timeSheet` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--timeSheet-patch` | PATCH `/timeSheet` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--timeSheet-post` | POST `/timeSheet` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--timeSheet-put` | PUT `/timeSheet` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--timeSheet--id--delete` | DELETE `/timeSheet/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--timeSheet--id--get` | GET `/timeSheet/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--timeSheet--id--patch` | PATCH `/timeSheet/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--timeSheet--id--put` | PUT `/timeSheet/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [timeSheet schemas](../schemas/timeSheet.md).

| Definition | Role |
| --- | --- |
| [`timeSheet`](../schemas/timeSheet.md#timesheet) | record body |
| [`timeSheetCollection`](../schemas/timeSheet.md#timesheetcollection) | collection page |
| [`timeSheetSelectOptions`](../schemas/timeSheet.md#timesheetselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
