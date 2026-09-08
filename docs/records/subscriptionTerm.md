# subscriptionTerm

Browser tag `subscriptionTerm` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/subscriptionTerm`, instance `/subscriptionTerm/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/subscriptionTerm` | `operation--subscriptionTerm-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/subscriptionTerm` | `operation--subscriptionTerm-get` | Get list of records. |  | 200 OK → `subscriptionTermCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/subscriptionTerm` | `operation--subscriptionTerm-patch` | Update records. | `subscriptionTermCollection` | 202 Accepted; default → `nsError` |
| POST | `/subscriptionTerm` | `operation--subscriptionTerm-post` | Insert record. | `subscriptionTerm` | 200 OK → `subscriptionTerm`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/subscriptionTerm` | `operation--subscriptionTerm-put` | Insert or update records. | `subscriptionTermCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/subscriptionTerm/{id}` | `operation--subscriptionTerm--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/subscriptionTerm/{id}` | `operation--subscriptionTerm--id--get` | Get record. |  | 200 OK → `subscriptionTerm`; 202 Accepted; default → `nsError` |
| PATCH | `/subscriptionTerm/{id}` | `operation--subscriptionTerm--id--patch` | Update record. | `subscriptionTerm` | 200 OK → `subscriptionTerm`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/subscriptionTerm/{id}` | `operation--subscriptionTerm--id--put` | Insert or update record. | `subscriptionTerm` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--subscriptionTerm-delete` | DELETE `/subscriptionTerm` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subscriptionTerm-get` | GET `/subscriptionTerm` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subscriptionTerm-patch` | PATCH `/subscriptionTerm` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subscriptionTerm-post` | POST `/subscriptionTerm` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--subscriptionTerm-put` | PUT `/subscriptionTerm` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subscriptionTerm--id--delete` | DELETE `/subscriptionTerm/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subscriptionTerm--id--get` | GET `/subscriptionTerm/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subscriptionTerm--id--patch` | PATCH `/subscriptionTerm/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--subscriptionTerm--id--put` | PUT `/subscriptionTerm/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [subscriptionTerm schemas](../schemas/subscriptionTerm.md).

| Definition | Role |
| --- | --- |
| [`subscriptionTerm`](../schemas/subscriptionTerm.md#subscriptionterm) | record body |
| [`subscriptionTermCollection`](../schemas/subscriptionTerm.md#subscriptiontermcollection) | collection page |
| [`subscriptionTermSelectOptions`](../schemas/subscriptionTerm.md#subscriptiontermselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
