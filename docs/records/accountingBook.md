# accountingBook

Browser tag `accountingBook` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/accountingBook`, instance `/accountingBook/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/accountingBook` | `operation--accountingBook-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/accountingBook` | `operation--accountingBook-get` | Get list of records. |  | 200 OK → `accountingBookCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/accountingBook` | `operation--accountingBook-patch` | Update records. | `accountingBookCollection` | 202 Accepted; default → `nsError` |
| POST | `/accountingBook` | `operation--accountingBook-post` | Insert record. | `accountingBook` | 200 OK → `accountingBook`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/accountingBook` | `operation--accountingBook-put` | Insert or update records. | `accountingBookCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/accountingBook/{id}` | `operation--accountingBook--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/accountingBook/{id}` | `operation--accountingBook--id--get` | Get record. |  | 200 OK → `accountingBook`; 202 Accepted; default → `nsError` |
| PATCH | `/accountingBook/{id}` | `operation--accountingBook--id--patch` | Update record. | `accountingBook` | 200 OK → `accountingBook`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/accountingBook/{id}` | `operation--accountingBook--id--put` | Insert or update record. | `accountingBook` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--accountingBook-delete` | DELETE `/accountingBook` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--accountingBook-get` | GET `/accountingBook` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--accountingBook-patch` | PATCH `/accountingBook` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--accountingBook-post` | POST `/accountingBook` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--accountingBook-put` | PUT `/accountingBook` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--accountingBook--id--delete` | DELETE `/accountingBook/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--accountingBook--id--get` | GET `/accountingBook/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--accountingBook--id--patch` | PATCH `/accountingBook/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--accountingBook--id--put` | PUT `/accountingBook/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [accountingBook schemas](../schemas/accountingBook.md).

| Definition | Role |
| --- | --- |
| [`accountingBook`](../schemas/accountingBook.md#accountingbook) | record body |
| [`accountingBook-accountingBookSubsidiariesCollection`](../schemas/accountingBook.md#accountingbook-accountingbooksubsidiariescollection) | sublist/collection |
| [`accountingBook-accountingBookSubsidiariesElement`](../schemas/accountingBook.md#accountingbook-accountingbooksubsidiarieselement) | sublist/element |
| [`accountingBookCollection`](../schemas/accountingBook.md#accountingbookcollection) | collection page |
| [`accountingBookSelectOptions`](../schemas/accountingBook.md#accountingbookselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookSubsidiaries` | [`accountingBook-accountingBookSubsidiariesCollection`](../schemas/accountingBook.md#accountingbook-accountingbooksubsidiariescollection) | [`accountingBook-accountingBookSubsidiariesElement`](../schemas/accountingBook.md#accountingbook-accountingbooksubsidiarieselement) |
