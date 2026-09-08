# taxSchedule

Browser tag `taxSchedule` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/taxSchedule`, instance `/taxSchedule/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/taxSchedule` | `operation--taxSchedule-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/taxSchedule` | `operation--taxSchedule-get` | Get list of records. |  | 200 OK → `taxScheduleCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/taxSchedule` | `operation--taxSchedule-patch` | Update records. | `taxScheduleCollection` | 202 Accepted; default → `nsError` |
| POST | `/taxSchedule` | `operation--taxSchedule-post` | Insert record. | `taxSchedule` | 200 OK → `taxSchedule`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/taxSchedule` | `operation--taxSchedule-put` | Insert or update records. | `taxScheduleCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/taxSchedule/{id}` | `operation--taxSchedule--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/taxSchedule/{id}` | `operation--taxSchedule--id--get` | Get record. |  | 200 OK → `taxSchedule`; 202 Accepted; default → `nsError` |
| PATCH | `/taxSchedule/{id}` | `operation--taxSchedule--id--patch` | Update record. | `taxSchedule` | 200 OK → `taxSchedule`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/taxSchedule/{id}` | `operation--taxSchedule--id--put` | Insert or update record. | `taxSchedule` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--taxSchedule-delete` | DELETE `/taxSchedule` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--taxSchedule-get` | GET `/taxSchedule` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--taxSchedule-patch` | PATCH `/taxSchedule` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--taxSchedule-post` | POST `/taxSchedule` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--taxSchedule-put` | PUT `/taxSchedule` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--taxSchedule--id--delete` | DELETE `/taxSchedule/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--taxSchedule--id--get` | GET `/taxSchedule/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--taxSchedule--id--patch` | PATCH `/taxSchedule/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--taxSchedule--id--put` | PUT `/taxSchedule/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [taxSchedule schemas](../schemas/taxSchedule.md).

| Definition | Role |
| --- | --- |
| [`taxSchedule`](../schemas/taxSchedule.md#taxschedule) | record body |
| [`taxSchedule-nexusesCollection`](../schemas/taxSchedule.md#taxschedule-nexusescollection) | sublist/collection |
| [`taxSchedule-nexusesElement`](../schemas/taxSchedule.md#taxschedule-nexuseselement) | sublist/element |
| [`taxSchedule-usNexusesCollection`](../schemas/taxSchedule.md#taxschedule-usnexusescollection) | sublist/collection |
| [`taxSchedule-usNexusesElement`](../schemas/taxSchedule.md#taxschedule-usnexuseselement) | sublist/element |
| [`taxScheduleCollection`](../schemas/taxSchedule.md#taxschedulecollection) | collection page |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `nexuses` | [`taxSchedule-nexusesCollection`](../schemas/taxSchedule.md#taxschedule-nexusescollection) | [`taxSchedule-nexusesElement`](../schemas/taxSchedule.md#taxschedule-nexuseselement) |
| `usNexuses` | [`taxSchedule-usNexusesCollection`](../schemas/taxSchedule.md#taxschedule-usnexusescollection) | [`taxSchedule-usNexusesElement`](../schemas/taxSchedule.md#taxschedule-usnexuseselement) |
