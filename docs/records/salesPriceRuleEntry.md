# salesPriceRuleEntry

Browser tag `salesPriceRuleEntry` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/salesPriceRuleEntry`, instance `/salesPriceRuleEntry/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/salesPriceRuleEntry` | `operation--salesPriceRuleEntry-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/salesPriceRuleEntry` | `operation--salesPriceRuleEntry-get` | Get list of records. |  | 200 OK → `salesPriceRuleEntryCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/salesPriceRuleEntry` | `operation--salesPriceRuleEntry-patch` | Update records. | `salesPriceRuleEntryCollection` | 202 Accepted; default → `nsError` |
| POST | `/salesPriceRuleEntry` | `operation--salesPriceRuleEntry-post` | Insert record. | `salesPriceRuleEntry` | 200 OK → `salesPriceRuleEntry`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/salesPriceRuleEntry` | `operation--salesPriceRuleEntry-put` | Insert or update records. | `salesPriceRuleEntryCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/salesPriceRuleEntry/{id}` | `operation--salesPriceRuleEntry--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/salesPriceRuleEntry/{id}` | `operation--salesPriceRuleEntry--id--get` | Get record. |  | 200 OK → `salesPriceRuleEntry`; 202 Accepted; default → `nsError` |
| PATCH | `/salesPriceRuleEntry/{id}` | `operation--salesPriceRuleEntry--id--patch` | Update record. | `salesPriceRuleEntry` | 200 OK → `salesPriceRuleEntry`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/salesPriceRuleEntry/{id}` | `operation--salesPriceRuleEntry--id--put` | Insert or update record. | `salesPriceRuleEntry` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--salesPriceRuleEntry-delete` | DELETE `/salesPriceRuleEntry` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--salesPriceRuleEntry-get` | GET `/salesPriceRuleEntry` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--salesPriceRuleEntry-patch` | PATCH `/salesPriceRuleEntry` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--salesPriceRuleEntry-post` | POST `/salesPriceRuleEntry` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--salesPriceRuleEntry-put` | PUT `/salesPriceRuleEntry` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--salesPriceRuleEntry--id--delete` | DELETE `/salesPriceRuleEntry/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--salesPriceRuleEntry--id--get` | GET `/salesPriceRuleEntry/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--salesPriceRuleEntry--id--patch` | PATCH `/salesPriceRuleEntry/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--salesPriceRuleEntry--id--put` | PUT `/salesPriceRuleEntry/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [salesPriceRuleEntry schemas](../schemas/salesPriceRuleEntry.md).

| Definition | Role |
| --- | --- |
| [`salesPriceRuleEntry`](../schemas/salesPriceRuleEntry.md#salespriceruleentry) | record body |
| [`salesPriceRuleEntryCollection`](../schemas/salesPriceRuleEntry.md#salespriceruleentrycollection) | collection page |
| [`salesPriceRuleEntrySelectOptions`](../schemas/salesPriceRuleEntry.md#salespriceruleentryselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
