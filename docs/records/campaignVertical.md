# campaignVertical

Browser tag `campaignVertical` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/campaignVertical`, instance `/campaignVertical/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/campaignVertical` | `operation--campaignVertical-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/campaignVertical` | `operation--campaignVertical-get` | Get list of records. |  | 200 OK → `campaignVerticalCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/campaignVertical` | `operation--campaignVertical-patch` | Update records. | `campaignVerticalCollection` | 202 Accepted; default → `nsError` |
| POST | `/campaignVertical` | `operation--campaignVertical-post` | Insert record. | `campaignVertical` | 200 OK → `campaignVertical`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/campaignVertical` | `operation--campaignVertical-put` | Insert or update records. | `campaignVerticalCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/campaignVertical/{id}` | `operation--campaignVertical--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/campaignVertical/{id}` | `operation--campaignVertical--id--get` | Get record. |  | 200 OK → `campaignVertical`; 202 Accepted; default → `nsError` |
| PATCH | `/campaignVertical/{id}` | `operation--campaignVertical--id--patch` | Update record. | `campaignVertical` | 200 OK → `campaignVertical`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/campaignVertical/{id}` | `operation--campaignVertical--id--put` | Insert or update record. | `campaignVertical` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--campaignVertical-delete` | DELETE `/campaignVertical` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignVertical-get` | GET `/campaignVertical` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignVertical-patch` | PATCH `/campaignVertical` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignVertical-post` | POST `/campaignVertical` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--campaignVertical-put` | PUT `/campaignVertical` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignVertical--id--delete` | DELETE `/campaignVertical/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignVertical--id--get` | GET `/campaignVertical/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignVertical--id--patch` | PATCH `/campaignVertical/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--campaignVertical--id--put` | PUT `/campaignVertical/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [campaignVertical schemas](../schemas/campaignVertical.md).

| Definition | Role |
| --- | --- |
| [`campaignVertical`](../schemas/campaignVertical.md#campaignvertical) | record body |
| [`campaignVerticalCollection`](../schemas/campaignVertical.md#campaignverticalcollection) | collection page |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
