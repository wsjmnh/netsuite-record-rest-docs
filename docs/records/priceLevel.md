# priceLevel

Browser tag `priceLevel` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/priceLevel`, instance `/priceLevel/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/priceLevel` | `operation--priceLevel-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/priceLevel` | `operation--priceLevel-get` | Get list of records. |  | 200 OK → `priceLevelCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/priceLevel` | `operation--priceLevel-patch` | Update records. | `priceLevelCollection` | 202 Accepted; default → `nsError` |
| POST | `/priceLevel` | `operation--priceLevel-post` | Insert record. | `priceLevel` | 200 OK → `priceLevel`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/priceLevel` | `operation--priceLevel-put` | Insert or update records. | `priceLevelCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/priceLevel/{id}` | `operation--priceLevel--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/priceLevel/{id}` | `operation--priceLevel--id--get` | Get record. |  | 200 OK → `priceLevel`; 202 Accepted; default → `nsError` |
| PATCH | `/priceLevel/{id}` | `operation--priceLevel--id--patch` | Update record. | `priceLevel` | 200 OK → `priceLevel`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/priceLevel/{id}` | `operation--priceLevel--id--put` | Insert or update record. | `priceLevel` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--priceLevel-delete` | DELETE `/priceLevel` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--priceLevel-get` | GET `/priceLevel` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--priceLevel-patch` | PATCH `/priceLevel` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--priceLevel-post` | POST `/priceLevel` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--priceLevel-put` | PUT `/priceLevel` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--priceLevel--id--delete` | DELETE `/priceLevel/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--priceLevel--id--get` | GET `/priceLevel/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--priceLevel--id--patch` | PATCH `/priceLevel/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--priceLevel--id--put` | PUT `/priceLevel/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [priceLevel schemas](../schemas/priceLevel.md).

| Definition | Role |
| --- | --- |
| [`priceLevel`](../schemas/priceLevel.md#pricelevel) | record body |
| [`priceLevelCollection`](../schemas/priceLevel.md#pricelevelcollection) | collection page |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
