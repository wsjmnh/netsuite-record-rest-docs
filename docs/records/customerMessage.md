# customerMessage

Browser tag `customerMessage` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/customerMessage`, instance `/customerMessage/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/customerMessage` | `operation--customerMessage-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/customerMessage` | `operation--customerMessage-get` | Get list of records. |  | 200 OK → `customerMessageCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/customerMessage` | `operation--customerMessage-patch` | Update records. | `customerMessageCollection` | 202 Accepted; default → `nsError` |
| POST | `/customerMessage` | `operation--customerMessage-post` | Insert record. | `customerMessage` | 200 OK → `customerMessage`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/customerMessage` | `operation--customerMessage-put` | Insert or update records. | `customerMessageCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/customerMessage/{id}` | `operation--customerMessage--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/customerMessage/{id}` | `operation--customerMessage--id--get` | Get record. |  | 200 OK → `customerMessage`; 202 Accepted; default → `nsError` |
| PATCH | `/customerMessage/{id}` | `operation--customerMessage--id--patch` | Update record. | `customerMessage` | 200 OK → `customerMessage`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/customerMessage/{id}` | `operation--customerMessage--id--put` | Insert or update record. | `customerMessage` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--customerMessage-delete` | DELETE `/customerMessage` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerMessage-get` | GET `/customerMessage` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerMessage-patch` | PATCH `/customerMessage` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerMessage-post` | POST `/customerMessage` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--customerMessage-put` | PUT `/customerMessage` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerMessage--id--delete` | DELETE `/customerMessage/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerMessage--id--get` | GET `/customerMessage/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerMessage--id--patch` | PATCH `/customerMessage/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--customerMessage--id--put` | PUT `/customerMessage/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [customerMessage schemas](../schemas/customerMessage.md).

| Definition | Role |
| --- | --- |
| [`customerMessage`](../schemas/customerMessage.md#customermessage) | record body |
| [`customerMessageCollection`](../schemas/customerMessage.md#customermessagecollection) | collection page |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
