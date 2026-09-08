# priceBook

Browser tag `priceBook` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/priceBook`, instance `/priceBook/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/priceBook` | `operation--priceBook-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/priceBook` | `operation--priceBook-get` | Get list of records. |  | 200 OK → `priceBookCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/priceBook` | `operation--priceBook-patch` | Update records. | `priceBookCollection` | 202 Accepted; default → `nsError` |
| POST | `/priceBook` | `operation--priceBook-post` | Insert record. | `priceBook` | 200 OK → `priceBook`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/priceBook` | `operation--priceBook-put` | Insert or update records. | `priceBookCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/priceBook/{id}` | `operation--priceBook--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/priceBook/{id}` | `operation--priceBook--id--get` | Get record. |  | 200 OK → `priceBook`; 202 Accepted; default → `nsError` |
| PATCH | `/priceBook/{id}` | `operation--priceBook--id--patch` | Update record. | `priceBook` | 200 OK → `priceBook`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/priceBook/{id}` | `operation--priceBook--id--put` | Insert or update record. | `priceBook` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--priceBook-delete` | DELETE `/priceBook` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--priceBook-get` | GET `/priceBook` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--priceBook-patch` | PATCH `/priceBook` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--priceBook-post` | POST `/priceBook` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--priceBook-put` | PUT `/priceBook` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--priceBook--id--delete` | DELETE `/priceBook/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--priceBook--id--get` | GET `/priceBook/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--priceBook--id--patch` | PATCH `/priceBook/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--priceBook--id--put` | PUT `/priceBook/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [priceBook schemas](../schemas/priceBook.md).

| Definition | Role |
| --- | --- |
| [`priceBook`](../schemas/priceBook.md#pricebook) | record body |
| [`priceBook-priceIntervalCollection`](../schemas/priceBook.md#pricebook-priceintervalcollection) | sublist/collection |
| [`priceBook-priceIntervalElement`](../schemas/priceBook.md#pricebook-priceintervalelement) | sublist/element |
| [`priceBookCollection`](../schemas/priceBook.md#pricebookcollection) | collection page |
| [`priceBookSelectOptions`](../schemas/priceBook.md#pricebookselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `priceInterval` | [`priceBook-priceIntervalCollection`](../schemas/priceBook.md#pricebook-priceintervalcollection) | [`priceBook-priceIntervalElement`](../schemas/priceBook.md#pricebook-priceintervalelement) |
