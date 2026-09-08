# campaignSearchEngine

Browser tag `campaignSearchEngine` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/campaignSearchEngine`, instance `/campaignSearchEngine/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/campaignSearchEngine` | `operation--campaignSearchEngine-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/campaignSearchEngine` | `operation--campaignSearchEngine-get` | Get list of records. |  | 200 OK → `campaignSearchEngineCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/campaignSearchEngine` | `operation--campaignSearchEngine-patch` | Update records. | `campaignSearchEngineCollection` | 202 Accepted; default → `nsError` |
| POST | `/campaignSearchEngine` | `operation--campaignSearchEngine-post` | Insert record. | `campaignSearchEngine` | 200 OK → `campaignSearchEngine`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/campaignSearchEngine` | `operation--campaignSearchEngine-put` | Insert or update records. | `campaignSearchEngineCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/campaignSearchEngine/{id}` | `operation--campaignSearchEngine--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/campaignSearchEngine/{id}` | `operation--campaignSearchEngine--id--get` | Get record. |  | 200 OK → `campaignSearchEngine`; 202 Accepted; default → `nsError` |
| PATCH | `/campaignSearchEngine/{id}` | `operation--campaignSearchEngine--id--patch` | Update record. | `campaignSearchEngine` | 200 OK → `campaignSearchEngine`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/campaignSearchEngine/{id}` | `operation--campaignSearchEngine--id--put` | Insert or update record. | `campaignSearchEngine` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--campaignSearchEngine-delete` | DELETE `/campaignSearchEngine` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignSearchEngine-get` | GET `/campaignSearchEngine` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignSearchEngine-patch` | PATCH `/campaignSearchEngine` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignSearchEngine-post` | POST `/campaignSearchEngine` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--campaignSearchEngine-put` | PUT `/campaignSearchEngine` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignSearchEngine--id--delete` | DELETE `/campaignSearchEngine/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignSearchEngine--id--get` | GET `/campaignSearchEngine/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignSearchEngine--id--patch` | PATCH `/campaignSearchEngine/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--campaignSearchEngine--id--put` | PUT `/campaignSearchEngine/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [campaignSearchEngine schemas](../schemas/campaignSearchEngine.md).

| Definition | Role |
| --- | --- |
| [`campaignSearchEngine`](../schemas/campaignSearchEngine.md#campaignsearchengine) | record body |
| [`campaignSearchEngineCollection`](../schemas/campaignSearchEngine.md#campaignsearchenginecollection) | collection page |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
