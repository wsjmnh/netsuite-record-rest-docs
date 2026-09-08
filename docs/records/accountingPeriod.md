# accountingPeriod

Browser tag `accountingPeriod` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/accountingPeriod`, instance `/accountingPeriod/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/accountingPeriod` | `operation--accountingPeriod-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/accountingPeriod` | `operation--accountingPeriod-get` | Get list of records. |  | 200 OK → `accountingPeriodCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/accountingPeriod` | `operation--accountingPeriod-patch` | Update records. | `accountingPeriodCollection` | 202 Accepted; default → `nsError` |
| POST | `/accountingPeriod` | `operation--accountingPeriod-post` | Insert record. | `accountingPeriod` | 200 OK → `accountingPeriod`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/accountingPeriod` | `operation--accountingPeriod-put` | Insert or update records. | `accountingPeriodCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/accountingPeriod/{id}` | `operation--accountingPeriod--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/accountingPeriod/{id}` | `operation--accountingPeriod--id--get` | Get record. |  | 200 OK → `accountingPeriod`; 202 Accepted; default → `nsError` |
| PATCH | `/accountingPeriod/{id}` | `operation--accountingPeriod--id--patch` | Update record. | `accountingPeriod` | 200 OK → `accountingPeriod`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/accountingPeriod/{id}` | `operation--accountingPeriod--id--put` | Insert or update record. | `accountingPeriod` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--accountingPeriod-delete` | DELETE `/accountingPeriod` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--accountingPeriod-get` | GET `/accountingPeriod` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--accountingPeriod-patch` | PATCH `/accountingPeriod` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--accountingPeriod-post` | POST `/accountingPeriod` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--accountingPeriod-put` | PUT `/accountingPeriod` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--accountingPeriod--id--delete` | DELETE `/accountingPeriod/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--accountingPeriod--id--get` | GET `/accountingPeriod/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--accountingPeriod--id--patch` | PATCH `/accountingPeriod/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--accountingPeriod--id--put` | PUT `/accountingPeriod/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [accountingPeriod schemas](../schemas/accountingPeriod.md).

| Definition | Role |
| --- | --- |
| [`accountingPeriod`](../schemas/accountingPeriod.md#accountingperiod) | record body |
| [`accountingPeriod-fiscalCalendarsCollection`](../schemas/accountingPeriod.md#accountingperiod-fiscalcalendarscollection) | sublist/collection |
| [`accountingPeriod-fiscalCalendarsElement`](../schemas/accountingPeriod.md#accountingperiod-fiscalcalendarselement) | sublist/element |
| [`accountingPeriod-perBookPeriodClosingCollection`](../schemas/accountingPeriod.md#accountingperiod-perbookperiodclosingcollection) | sublist/collection |
| [`accountingPeriod-perBookPeriodClosingElement`](../schemas/accountingPeriod.md#accountingperiod-perbookperiodclosingelement) | sublist/element |
| [`accountingPeriodCollection`](../schemas/accountingPeriod.md#accountingperiodcollection) | collection page |
| [`accountingPeriodSelectOptions`](../schemas/accountingPeriod.md#accountingperiodselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `fiscalCalendars` | [`accountingPeriod-fiscalCalendarsCollection`](../schemas/accountingPeriod.md#accountingperiod-fiscalcalendarscollection) | [`accountingPeriod-fiscalCalendarsElement`](../schemas/accountingPeriod.md#accountingperiod-fiscalcalendarselement) |
| `perBookPeriodClosing` | [`accountingPeriod-perBookPeriodClosingCollection`](../schemas/accountingPeriod.md#accountingperiod-perbookperiodclosingcollection) | [`accountingPeriod-perBookPeriodClosingElement`](../schemas/accountingPeriod.md#accountingperiod-perbookperiodclosingelement) |
