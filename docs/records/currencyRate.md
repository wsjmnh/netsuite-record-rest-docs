# currencyRate

Browser tag `currencyRate` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/currencyRate`, instance `/currencyRate/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| GET | `/currencyRate` | `operation--currencyRate-get` | Get list of records. |  | 200 OK → `currencyRateCollection`; 202 Accepted; default → `nsError` |
| POST | `/currencyRate` | `operation--currencyRate-post` | Insert record. | `currencyRate` | 200 OK → `currencyRate`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/currencyRate` | `operation--currencyRate-put` | Insert or update records. | `currencyRateCollection` | 202 Accepted; default → `nsError` |
| GET | `/currencyRate/{id}` | `operation--currencyRate--id--get` | Get record. |  | 200 OK → `currencyRate`; 202 Accepted; default → `nsError` |
| PUT | `/currencyRate/{id}` | `operation--currencyRate--id--put` | Insert or update record. | `currencyRate` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--currencyRate-get` | GET `/currencyRate` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--currencyRate-post` | POST `/currencyRate` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--currencyRate-put` | PUT `/currencyRate` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--currencyRate--id--get` | GET `/currencyRate/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--currencyRate--id--put` | PUT `/currencyRate/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [currencyRate schemas](../schemas/currencyRate.md).

| Definition | Role |
| --- | --- |
| [`currencyRate`](../schemas/currencyRate.md#currencyrate) | record body |
| [`currencyRateCollection`](../schemas/currencyRate.md#currencyratecollection) | collection page |
| [`currencyRateSelectOptions`](../schemas/currencyRate.md#currencyrateselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
