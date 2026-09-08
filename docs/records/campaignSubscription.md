# campaignSubscription

Browser tag `campaignSubscription` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/campaignSubscription`, instance `/campaignSubscription/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/campaignSubscription` | `operation--campaignSubscription-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/campaignSubscription` | `operation--campaignSubscription-get` | Get list of records. |  | 200 OK → `campaignSubscriptionCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/campaignSubscription` | `operation--campaignSubscription-patch` | Update records. | `campaignSubscriptionCollection` | 202 Accepted; default → `nsError` |
| POST | `/campaignSubscription` | `operation--campaignSubscription-post` | Insert record. | `campaignSubscription` | 200 OK → `campaignSubscription`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/campaignSubscription` | `operation--campaignSubscription-put` | Insert or update records. | `campaignSubscriptionCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/campaignSubscription/{id}` | `operation--campaignSubscription--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/campaignSubscription/{id}` | `operation--campaignSubscription--id--get` | Get record. |  | 200 OK → `campaignSubscription`; 202 Accepted; default → `nsError` |
| PATCH | `/campaignSubscription/{id}` | `operation--campaignSubscription--id--patch` | Update record. | `campaignSubscription` | 200 OK → `campaignSubscription`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/campaignSubscription/{id}` | `operation--campaignSubscription--id--put` | Insert or update record. | `campaignSubscription` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--campaignSubscription-delete` | DELETE `/campaignSubscription` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignSubscription-get` | GET `/campaignSubscription` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignSubscription-patch` | PATCH `/campaignSubscription` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignSubscription-post` | POST `/campaignSubscription` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--campaignSubscription-put` | PUT `/campaignSubscription` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignSubscription--id--delete` | DELETE `/campaignSubscription/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignSubscription--id--get` | GET `/campaignSubscription/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignSubscription--id--patch` | PATCH `/campaignSubscription/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--campaignSubscription--id--put` | PUT `/campaignSubscription/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [campaignSubscription schemas](../schemas/campaignSubscription.md).

| Definition | Role |
| --- | --- |
| [`campaignSubscription`](../schemas/campaignSubscription.md#campaignsubscription) | record body |
| [`campaignSubscriptionCollection`](../schemas/campaignSubscription.md#campaignsubscriptioncollection) | collection page |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
