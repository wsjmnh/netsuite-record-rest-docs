# campaignFamily

Browser tag `campaignFamily` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/campaignFamily`, instance `/campaignFamily/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/campaignFamily` | `operation--campaignFamily-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/campaignFamily` | `operation--campaignFamily-get` | Get list of records. |  | 200 OK → `campaignFamilyCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/campaignFamily` | `operation--campaignFamily-patch` | Update records. | `campaignFamilyCollection` | 202 Accepted; default → `nsError` |
| POST | `/campaignFamily` | `operation--campaignFamily-post` | Insert record. | `campaignFamily` | 200 OK → `campaignFamily`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/campaignFamily` | `operation--campaignFamily-put` | Insert or update records. | `campaignFamilyCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/campaignFamily/{id}` | `operation--campaignFamily--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/campaignFamily/{id}` | `operation--campaignFamily--id--get` | Get record. |  | 200 OK → `campaignFamily`; 202 Accepted; default → `nsError` |
| PATCH | `/campaignFamily/{id}` | `operation--campaignFamily--id--patch` | Update record. | `campaignFamily` | 200 OK → `campaignFamily`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/campaignFamily/{id}` | `operation--campaignFamily--id--put` | Insert or update record. | `campaignFamily` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--campaignFamily-delete` | DELETE `/campaignFamily` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignFamily-get` | GET `/campaignFamily` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignFamily-patch` | PATCH `/campaignFamily` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignFamily-post` | POST `/campaignFamily` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--campaignFamily-put` | PUT `/campaignFamily` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignFamily--id--delete` | DELETE `/campaignFamily/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignFamily--id--get` | GET `/campaignFamily/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignFamily--id--patch` | PATCH `/campaignFamily/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--campaignFamily--id--put` | PUT `/campaignFamily/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [campaignFamily schemas](../schemas/campaignFamily.md).

| Definition | Role |
| --- | --- |
| [`campaignFamily`](../schemas/campaignFamily.md#campaignfamily) | record body |
| [`campaignFamilyCollection`](../schemas/campaignFamily.md#campaignfamilycollection) | collection page |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
