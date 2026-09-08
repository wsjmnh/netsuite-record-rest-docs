# winLossReason

Browser tag `winLossReason` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/winLossReason`, instance `/winLossReason/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/winLossReason` | `operation--winLossReason-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/winLossReason` | `operation--winLossReason-get` | Get list of records. |  | 200 OK → `winLossReasonCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/winLossReason` | `operation--winLossReason-patch` | Update records. | `winLossReasonCollection` | 202 Accepted; default → `nsError` |
| POST | `/winLossReason` | `operation--winLossReason-post` | Insert record. | `winLossReason` | 200 OK → `winLossReason`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/winLossReason` | `operation--winLossReason-put` | Insert or update records. | `winLossReasonCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/winLossReason/{id}` | `operation--winLossReason--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/winLossReason/{id}` | `operation--winLossReason--id--get` | Get record. |  | 200 OK → `winLossReason`; 202 Accepted; default → `nsError` |
| PATCH | `/winLossReason/{id}` | `operation--winLossReason--id--patch` | Update record. | `winLossReason` | 200 OK → `winLossReason`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/winLossReason/{id}` | `operation--winLossReason--id--put` | Insert or update record. | `winLossReason` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--winLossReason-delete` | DELETE `/winLossReason` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--winLossReason-get` | GET `/winLossReason` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--winLossReason-patch` | PATCH `/winLossReason` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--winLossReason-post` | POST `/winLossReason` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--winLossReason-put` | PUT `/winLossReason` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--winLossReason--id--delete` | DELETE `/winLossReason/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--winLossReason--id--get` | GET `/winLossReason/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--winLossReason--id--patch` | PATCH `/winLossReason/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--winLossReason--id--put` | PUT `/winLossReason/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [winLossReason schemas](../schemas/winLossReason.md).

| Definition | Role |
| --- | --- |
| [`winLossReason`](../schemas/winLossReason.md#winlossreason) | record body |
| [`winLossReasonCollection`](../schemas/winLossReason.md#winlossreasoncollection) | collection page |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
