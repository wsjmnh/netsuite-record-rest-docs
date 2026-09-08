# revRecSchedule

Browser tag `revRecSchedule` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/revRecSchedule`, instance `/revRecSchedule/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| GET | `/revRecSchedule` | `operation--revRecSchedule-get` | Get list of records. |  | 200 OK → `revRecScheduleCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/revRecSchedule` | `operation--revRecSchedule-patch` | Update records. | `revRecScheduleCollection` | 202 Accepted; default → `nsError` |
| POST | `/revRecSchedule` | `operation--revRecSchedule-post` | Insert record. | `revRecSchedule` | 200 OK → `revRecSchedule`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/revRecSchedule` | `operation--revRecSchedule-put` | Insert or update records. | `revRecScheduleCollection` | 202 Accepted; default → `nsError` |
| GET | `/revRecSchedule/{id}` | `operation--revRecSchedule--id--get` | Get record. |  | 200 OK → `revRecSchedule`; 202 Accepted; default → `nsError` |
| PATCH | `/revRecSchedule/{id}` | `operation--revRecSchedule--id--patch` | Update record. | `revRecSchedule` | 200 OK → `revRecSchedule`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/revRecSchedule/{id}` | `operation--revRecSchedule--id--put` | Insert or update record. | `revRecSchedule` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--revRecSchedule-get` | GET `/revRecSchedule` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--revRecSchedule-patch` | PATCH `/revRecSchedule` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--revRecSchedule-post` | POST `/revRecSchedule` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--revRecSchedule-put` | PUT `/revRecSchedule` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--revRecSchedule--id--get` | GET `/revRecSchedule/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--revRecSchedule--id--patch` | PATCH `/revRecSchedule/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--revRecSchedule--id--put` | PUT `/revRecSchedule/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [revRecSchedule schemas](../schemas/revRecSchedule.md).

| Definition | Role |
| --- | --- |
| [`revRecSchedule`](../schemas/revRecSchedule.md#revrecschedule) | record body |
| [`revRecSchedule-recurrenceCollection`](../schemas/revRecSchedule.md#revrecschedule-recurrencecollection) | sublist/collection |
| [`revRecSchedule-recurrenceElement`](../schemas/revRecSchedule.md#revrecschedule-recurrenceelement) | sublist/element |
| [`revRecScheduleCollection`](../schemas/revRecSchedule.md#revrecschedulecollection) | collection page |
| [`revRecScheduleSelectOptions`](../schemas/revRecSchedule.md#revrecscheduleselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `recurrence` | [`revRecSchedule-recurrenceCollection`](../schemas/revRecSchedule.md#revrecschedule-recurrencecollection) | [`revRecSchedule-recurrenceElement`](../schemas/revRecSchedule.md#revrecschedule-recurrenceelement) |
