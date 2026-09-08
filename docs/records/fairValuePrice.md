# fairValuePrice

Browser tag `fairValuePrice` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/fairValuePrice`, instance `/fairValuePrice/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/fairValuePrice` | `operation--fairValuePrice-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/fairValuePrice` | `operation--fairValuePrice-get` | Get list of records. |  | 200 OK → `fairValuePriceCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/fairValuePrice` | `operation--fairValuePrice-patch` | Update records. | `fairValuePriceCollection` | 202 Accepted; default → `nsError` |
| POST | `/fairValuePrice` | `operation--fairValuePrice-post` | Insert record. | `fairValuePrice` | 200 OK → `fairValuePrice`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/fairValuePrice` | `operation--fairValuePrice-put` | Insert or update records. | `fairValuePriceCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/fairValuePrice/{id}` | `operation--fairValuePrice--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/fairValuePrice/{id}` | `operation--fairValuePrice--id--get` | Get record. |  | 200 OK → `fairValuePrice`; 202 Accepted; default → `nsError` |
| PATCH | `/fairValuePrice/{id}` | `operation--fairValuePrice--id--patch` | Update record. | `fairValuePrice` | 200 OK → `fairValuePrice`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/fairValuePrice/{id}` | `operation--fairValuePrice--id--put` | Insert or update record. | `fairValuePrice` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--fairValuePrice-delete` | DELETE `/fairValuePrice` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--fairValuePrice-get` | GET `/fairValuePrice` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--fairValuePrice-patch` | PATCH `/fairValuePrice` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--fairValuePrice-post` | POST `/fairValuePrice` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--fairValuePrice-put` | PUT `/fairValuePrice` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--fairValuePrice--id--delete` | DELETE `/fairValuePrice/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--fairValuePrice--id--get` | GET `/fairValuePrice/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--fairValuePrice--id--patch` | PATCH `/fairValuePrice/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--fairValuePrice--id--put` | PUT `/fairValuePrice/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [fairValuePrice schemas](../schemas/fairValuePrice.md).

| Definition | Role |
| --- | --- |
| [`fairValuePrice`](../schemas/fairValuePrice.md#fairvalueprice) | record body |
| [`fairValuePriceCollection`](../schemas/fairValuePrice.md#fairvaluepricecollection) | collection page |
| [`fairValuePriceSelectOptions`](../schemas/fairValuePrice.md#fairvaluepriceselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
