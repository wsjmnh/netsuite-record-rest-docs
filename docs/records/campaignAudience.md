# campaignAudience

Browser tag `campaignAudience` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/campaignAudience`, instance `/campaignAudience/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/campaignAudience` | `operation--campaignAudience-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/campaignAudience` | `operation--campaignAudience-get` | Get list of records. |  | 200 OK → `campaignAudienceCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/campaignAudience` | `operation--campaignAudience-patch` | Update records. | `campaignAudienceCollection` | 202 Accepted; default → `nsError` |
| POST | `/campaignAudience` | `operation--campaignAudience-post` | Insert record. | `campaignAudience` | 200 OK → `campaignAudience`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/campaignAudience` | `operation--campaignAudience-put` | Insert or update records. | `campaignAudienceCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/campaignAudience/{id}` | `operation--campaignAudience--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/campaignAudience/{id}` | `operation--campaignAudience--id--get` | Get record. |  | 200 OK → `campaignAudience`; 202 Accepted; default → `nsError` |
| PATCH | `/campaignAudience/{id}` | `operation--campaignAudience--id--patch` | Update record. | `campaignAudience` | 200 OK → `campaignAudience`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/campaignAudience/{id}` | `operation--campaignAudience--id--put` | Insert or update record. | `campaignAudience` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--campaignAudience-delete` | DELETE `/campaignAudience` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignAudience-get` | GET `/campaignAudience` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignAudience-patch` | PATCH `/campaignAudience` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignAudience-post` | POST `/campaignAudience` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--campaignAudience-put` | PUT `/campaignAudience` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignAudience--id--delete` | DELETE `/campaignAudience/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignAudience--id--get` | GET `/campaignAudience/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignAudience--id--patch` | PATCH `/campaignAudience/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--campaignAudience--id--put` | PUT `/campaignAudience/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [campaignAudience schemas](../schemas/campaignAudience.md).

| Definition | Role |
| --- | --- |
| [`campaignAudience`](../schemas/campaignAudience.md#campaignaudience) | record body |
| [`campaignAudienceCollection`](../schemas/campaignAudience.md#campaignaudiencecollection) | collection page |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
