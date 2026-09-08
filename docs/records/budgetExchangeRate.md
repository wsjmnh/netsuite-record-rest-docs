# budgetExchangeRate

Browser tag `budgetExchangeRate` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/budgetExchangeRate`, instance `/budgetExchangeRate/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| GET | `/budgetExchangeRate` | `operation--budgetExchangeRate-get` | Get list of records. |  | 200 OK → `budgetExchangeRateCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/budgetExchangeRate` | `operation--budgetExchangeRate-patch` | Update records. | `budgetExchangeRateCollection` | 202 Accepted; default → `nsError` |
| PUT | `/budgetExchangeRate` | `operation--budgetExchangeRate-put` | Insert or update records. | `budgetExchangeRateCollection` | 202 Accepted; default → `nsError` |
| GET | `/budgetExchangeRate/{id}` | `operation--budgetExchangeRate--id--get` | Get record. |  | 200 OK → `budgetExchangeRate`; 202 Accepted; default → `nsError` |
| PATCH | `/budgetExchangeRate/{id}` | `operation--budgetExchangeRate--id--patch` | Update record. | `budgetExchangeRate` | 200 OK → `budgetExchangeRate`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/budgetExchangeRate/{id}` | `operation--budgetExchangeRate--id--put` | Insert or update record. | `budgetExchangeRate` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--budgetExchangeRate-get` | GET `/budgetExchangeRate` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--budgetExchangeRate-patch` | PATCH `/budgetExchangeRate` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--budgetExchangeRate-put` | PUT `/budgetExchangeRate` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--budgetExchangeRate--id--get` | GET `/budgetExchangeRate/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--budgetExchangeRate--id--patch` | PATCH `/budgetExchangeRate/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--budgetExchangeRate--id--put` | PUT `/budgetExchangeRate/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [budgetExchangeRate schemas](../schemas/budgetExchangeRate.md).

| Definition | Role |
| --- | --- |
| [`budgetExchangeRate`](../schemas/budgetExchangeRate.md#budgetexchangerate) | record body |
| [`budgetExchangeRateCollection`](../schemas/budgetExchangeRate.md#budgetexchangeratecollection) | collection page |
| [`budgetExchangeRateSelectOptions`](../schemas/budgetExchangeRate.md#budgetexchangerateselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
