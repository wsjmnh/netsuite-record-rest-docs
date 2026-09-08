# billingRevenueEvent

Browser tag `billingRevenueEvent` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/billingRevenueEvent`, instance `/billingRevenueEvent/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/billingRevenueEvent` | `operation--billingRevenueEvent-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/billingRevenueEvent` | `operation--billingRevenueEvent-get` | Get list of records. |  | 200 OK → `billingRevenueEventCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/billingRevenueEvent` | `operation--billingRevenueEvent-patch` | Update records. | `billingRevenueEventCollection` | 202 Accepted; default → `nsError` |
| POST | `/billingRevenueEvent` | `operation--billingRevenueEvent-post` | Insert record. | `billingRevenueEvent` | 200 OK → `billingRevenueEvent`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/billingRevenueEvent` | `operation--billingRevenueEvent-put` | Insert or update records. | `billingRevenueEventCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/billingRevenueEvent/{id}` | `operation--billingRevenueEvent--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/billingRevenueEvent/{id}` | `operation--billingRevenueEvent--id--get` | Get record. |  | 200 OK → `billingRevenueEvent`; 202 Accepted; default → `nsError` |
| PATCH | `/billingRevenueEvent/{id}` | `operation--billingRevenueEvent--id--patch` | Update record. | `billingRevenueEvent` | 200 OK → `billingRevenueEvent`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/billingRevenueEvent/{id}` | `operation--billingRevenueEvent--id--put` | Insert or update record. | `billingRevenueEvent` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--billingRevenueEvent-delete` | DELETE `/billingRevenueEvent` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--billingRevenueEvent-get` | GET `/billingRevenueEvent` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--billingRevenueEvent-patch` | PATCH `/billingRevenueEvent` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--billingRevenueEvent-post` | POST `/billingRevenueEvent` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--billingRevenueEvent-put` | PUT `/billingRevenueEvent` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--billingRevenueEvent--id--delete` | DELETE `/billingRevenueEvent/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--billingRevenueEvent--id--get` | GET `/billingRevenueEvent/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--billingRevenueEvent--id--patch` | PATCH `/billingRevenueEvent/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--billingRevenueEvent--id--put` | PUT `/billingRevenueEvent/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [billingRevenueEvent schemas](../schemas/billingRevenueEvent.md).

| Definition | Role |
| --- | --- |
| [`billingRevenueEvent`](../schemas/billingRevenueEvent.md#billingrevenueevent) | record body |
| [`billingRevenueEventCollection`](../schemas/billingRevenueEvent.md#billingrevenueeventcollection) | collection page |
| [`billingRevenueEventSelectOptions`](../schemas/billingRevenueEvent.md#billingrevenueeventselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
