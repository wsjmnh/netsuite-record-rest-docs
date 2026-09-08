# campaignOffer

Browser tag `campaignOffer` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/campaignOffer`, instance `/campaignOffer/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/campaignOffer` | `operation--campaignOffer-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/campaignOffer` | `operation--campaignOffer-get` | Get list of records. |  | 200 OK → `campaignOfferCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/campaignOffer` | `operation--campaignOffer-patch` | Update records. | `campaignOfferCollection` | 202 Accepted; default → `nsError` |
| POST | `/campaignOffer` | `operation--campaignOffer-post` | Insert record. | `campaignOffer` | 200 OK → `campaignOffer`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/campaignOffer` | `operation--campaignOffer-put` | Insert or update records. | `campaignOfferCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/campaignOffer/{id}` | `operation--campaignOffer--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/campaignOffer/{id}` | `operation--campaignOffer--id--get` | Get record. |  | 200 OK → `campaignOffer`; 202 Accepted; default → `nsError` |
| PATCH | `/campaignOffer/{id}` | `operation--campaignOffer--id--patch` | Update record. | `campaignOffer` | 200 OK → `campaignOffer`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/campaignOffer/{id}` | `operation--campaignOffer--id--put` | Insert or update record. | `campaignOffer` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--campaignOffer-delete` | DELETE `/campaignOffer` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignOffer-get` | GET `/campaignOffer` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignOffer-patch` | PATCH `/campaignOffer` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignOffer-post` | POST `/campaignOffer` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--campaignOffer-put` | PUT `/campaignOffer` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignOffer--id--delete` | DELETE `/campaignOffer/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignOffer--id--get` | GET `/campaignOffer/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignOffer--id--patch` | PATCH `/campaignOffer/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--campaignOffer--id--put` | PUT `/campaignOffer/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [campaignOffer schemas](../schemas/campaignOffer.md).

| Definition | Role |
| --- | --- |
| [`campaignOffer`](../schemas/campaignOffer.md#campaignoffer) | record body |
| [`campaignOfferCollection`](../schemas/campaignOffer.md#campaignoffercollection) | collection page |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
