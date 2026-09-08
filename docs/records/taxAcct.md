# taxAcct

Browser tag `taxAcct` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/taxAcct`, instance `/taxAcct/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/taxAcct` | `operation--taxAcct-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/taxAcct` | `operation--taxAcct-get` | Get list of records. |  | 200 OK → `taxAcctCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/taxAcct` | `operation--taxAcct-patch` | Update records. | `taxAcctCollection` | 202 Accepted; default → `nsError` |
| POST | `/taxAcct` | `operation--taxAcct-post` | Insert record. | `taxAcct` | 200 OK → `taxAcct`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/taxAcct` | `operation--taxAcct-put` | Insert or update records. | `taxAcctCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/taxAcct/{id}` | `operation--taxAcct--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/taxAcct/{id}` | `operation--taxAcct--id--get` | Get record. |  | 200 OK → `taxAcct`; 202 Accepted; default → `nsError` |
| PATCH | `/taxAcct/{id}` | `operation--taxAcct--id--patch` | Update record. | `taxAcct` | 200 OK → `taxAcct`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/taxAcct/{id}` | `operation--taxAcct--id--put` | Insert or update record. | `taxAcct` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--taxAcct-delete` | DELETE `/taxAcct` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--taxAcct-get` | GET `/taxAcct` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--taxAcct-patch` | PATCH `/taxAcct` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--taxAcct-post` | POST `/taxAcct` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--taxAcct-put` | PUT `/taxAcct` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--taxAcct--id--delete` | DELETE `/taxAcct/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--taxAcct--id--get` | GET `/taxAcct/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--taxAcct--id--patch` | PATCH `/taxAcct/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--taxAcct--id--put` | PUT `/taxAcct/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [taxAcct schemas](../schemas/taxAcct.md).

| Definition | Role |
| --- | --- |
| [`taxAcct`](../schemas/taxAcct.md#taxacct) | record body |
| [`taxAcctCollection`](../schemas/taxAcct.md#taxacctcollection) | collection page |
| [`taxAcctSelectOptions`](../schemas/taxAcct.md#taxacctselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
