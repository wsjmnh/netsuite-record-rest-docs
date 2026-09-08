# paymentCard

Browser tag `paymentCard` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/paymentCard`, instance `/paymentCard/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/paymentCard` | `operation--paymentCard-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/paymentCard` | `operation--paymentCard-get` | Get list of records. |  | 200 OK → `paymentCardCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/paymentCard` | `operation--paymentCard-patch` | Update records. | `paymentCardCollection` | 202 Accepted; default → `nsError` |
| POST | `/paymentCard` | `operation--paymentCard-post` | Insert record. | `paymentCard` | 200 OK → `paymentCard`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/paymentCard` | `operation--paymentCard-put` | Insert or update records. | `paymentCardCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/paymentCard/{id}` | `operation--paymentCard--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/paymentCard/{id}` | `operation--paymentCard--id--get` | Get record. |  | 200 OK → `paymentCard`; 202 Accepted; default → `nsError` |
| PATCH | `/paymentCard/{id}` | `operation--paymentCard--id--patch` | Update record. | `paymentCard` | 200 OK → `paymentCard`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/paymentCard/{id}` | `operation--paymentCard--id--put` | Insert or update record. | `paymentCard` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--paymentCard-delete` | DELETE `/paymentCard` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--paymentCard-get` | GET `/paymentCard` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--paymentCard-patch` | PATCH `/paymentCard` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--paymentCard-post` | POST `/paymentCard` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--paymentCard-put` | PUT `/paymentCard` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--paymentCard--id--delete` | DELETE `/paymentCard/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--paymentCard--id--get` | GET `/paymentCard/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--paymentCard--id--patch` | PATCH `/paymentCard/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--paymentCard--id--put` | PUT `/paymentCard/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [paymentCard schemas](../schemas/paymentCard.md).

| Definition | Role |
| --- | --- |
| [`paymentCard`](../schemas/paymentCard.md#paymentcard) | record body |
| [`paymentCardCollection`](../schemas/paymentCard.md#paymentcardcollection) | collection page |
| [`paymentCardSelectOptions`](../schemas/paymentCard.md#paymentcardselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
