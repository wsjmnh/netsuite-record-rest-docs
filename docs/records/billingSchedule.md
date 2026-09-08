# billingSchedule

Browser tag `billingSchedule` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/billingSchedule`, instance `/billingSchedule/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/billingSchedule` | `operation--billingSchedule-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/billingSchedule` | `operation--billingSchedule-get` | Get list of records. |  | 200 OK → `billingScheduleCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/billingSchedule` | `operation--billingSchedule-patch` | Update records. | `billingScheduleCollection` | 202 Accepted; default → `nsError` |
| POST | `/billingSchedule` | `operation--billingSchedule-post` | Insert record. | `billingSchedule` | 200 OK → `billingSchedule`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/billingSchedule` | `operation--billingSchedule-put` | Insert or update records. | `billingScheduleCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/billingSchedule/{id}` | `operation--billingSchedule--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/billingSchedule/{id}` | `operation--billingSchedule--id--get` | Get record. |  | 200 OK → `billingSchedule`; 202 Accepted; default → `nsError` |
| PATCH | `/billingSchedule/{id}` | `operation--billingSchedule--id--patch` | Update record. | `billingSchedule` | 200 OK → `billingSchedule`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/billingSchedule/{id}` | `operation--billingSchedule--id--put` | Insert or update record. | `billingSchedule` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--billingSchedule-delete` | DELETE `/billingSchedule` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--billingSchedule-get` | GET `/billingSchedule` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--billingSchedule-patch` | PATCH `/billingSchedule` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--billingSchedule-post` | POST `/billingSchedule` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--billingSchedule-put` | PUT `/billingSchedule` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--billingSchedule--id--delete` | DELETE `/billingSchedule/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--billingSchedule--id--get` | GET `/billingSchedule/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--billingSchedule--id--patch` | PATCH `/billingSchedule/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--billingSchedule--id--put` | PUT `/billingSchedule/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [billingSchedule schemas](../schemas/billingSchedule.md).

| Definition | Role |
| --- | --- |
| [`billingSchedule`](../schemas/billingSchedule.md#billingschedule) | record body |
| [`billingSchedule-milestoneCollection`](../schemas/billingSchedule.md#billingschedule-milestonecollection) | sublist/collection |
| [`billingSchedule-milestoneElement`](../schemas/billingSchedule.md#billingschedule-milestoneelement) | sublist/element |
| [`billingSchedule-recurrenceCollection`](../schemas/billingSchedule.md#billingschedule-recurrencecollection) | sublist/collection |
| [`billingSchedule-recurrenceElement`](../schemas/billingSchedule.md#billingschedule-recurrenceelement) | sublist/element |
| [`billingScheduleCollection`](../schemas/billingSchedule.md#billingschedulecollection) | collection page |
| [`billingScheduleSelectOptions`](../schemas/billingSchedule.md#billingscheduleselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `milestone` | [`billingSchedule-milestoneCollection`](../schemas/billingSchedule.md#billingschedule-milestonecollection) | [`billingSchedule-milestoneElement`](../schemas/billingSchedule.md#billingschedule-milestoneelement) |
| `recurrence` | [`billingSchedule-recurrenceCollection`](../schemas/billingSchedule.md#billingschedule-recurrencecollection) | [`billingSchedule-recurrenceElement`](../schemas/billingSchedule.md#billingschedule-recurrenceelement) |
