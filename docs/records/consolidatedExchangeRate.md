# consolidatedExchangeRate

Browser tag `consolidatedExchangeRate` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/consolidatedExchangeRate`, instance `/consolidatedExchangeRate/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| GET | `/consolidatedExchangeRate` | `operation--consolidatedExchangeRate-get` | Get list of records. |  | 200 OK → `consolidatedExchangeRateCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/consolidatedExchangeRate` | `operation--consolidatedExchangeRate-patch` | Update records. | `consolidatedExchangeRateCollection` | 202 Accepted; default → `nsError` |
| PUT | `/consolidatedExchangeRate` | `operation--consolidatedExchangeRate-put` | Insert or update records. | `consolidatedExchangeRateCollection` | 202 Accepted; default → `nsError` |
| GET | `/consolidatedExchangeRate/{id}` | `operation--consolidatedExchangeRate--id--get` | Get record. |  | 200 OK → `consolidatedExchangeRate`; 202 Accepted; default → `nsError` |
| PATCH | `/consolidatedExchangeRate/{id}` | `operation--consolidatedExchangeRate--id--patch` | Update record. | `consolidatedExchangeRate` | 200 OK → `consolidatedExchangeRate`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/consolidatedExchangeRate/{id}` | `operation--consolidatedExchangeRate--id--put` | Insert or update record. | `consolidatedExchangeRate` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--consolidatedExchangeRate-get` | GET `/consolidatedExchangeRate` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--consolidatedExchangeRate-patch` | PATCH `/consolidatedExchangeRate` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--consolidatedExchangeRate-put` | PUT `/consolidatedExchangeRate` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--consolidatedExchangeRate--id--get` | GET `/consolidatedExchangeRate/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--consolidatedExchangeRate--id--patch` | PATCH `/consolidatedExchangeRate/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--consolidatedExchangeRate--id--put` | PUT `/consolidatedExchangeRate/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [consolidatedExchangeRate schemas](../schemas/consolidatedExchangeRate.md).

| Definition | Role |
| --- | --- |
| [`consolidatedExchangeRate`](../schemas/consolidatedExchangeRate.md#consolidatedexchangerate) | record body |
| [`consolidatedExchangeRateCollection`](../schemas/consolidatedExchangeRate.md#consolidatedexchangeratecollection) | collection page |
| [`consolidatedExchangeRateSelectOptions`](../schemas/consolidatedExchangeRate.md#consolidatedexchangerateselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
