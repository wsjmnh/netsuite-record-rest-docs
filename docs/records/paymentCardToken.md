# paymentCardToken

Browser tag `paymentCardToken` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/paymentCardToken`, instance `/paymentCardToken/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/paymentCardToken` | `operation--paymentCardToken-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/paymentCardToken` | `operation--paymentCardToken-get` | Get list of records. |  | 200 OK → `paymentCardTokenCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/paymentCardToken` | `operation--paymentCardToken-patch` | Update records. | `paymentCardTokenCollection` | 202 Accepted; default → `nsError` |
| POST | `/paymentCardToken` | `operation--paymentCardToken-post` | Insert record. | `paymentCardToken` | 200 OK → `paymentCardToken`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/paymentCardToken` | `operation--paymentCardToken-put` | Insert or update records. | `paymentCardTokenCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/paymentCardToken/{id}` | `operation--paymentCardToken--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/paymentCardToken/{id}` | `operation--paymentCardToken--id--get` | Get record. |  | 200 OK → `paymentCardToken`; 202 Accepted; default → `nsError` |
| PATCH | `/paymentCardToken/{id}` | `operation--paymentCardToken--id--patch` | Update record. | `paymentCardToken` | 200 OK → `paymentCardToken`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/paymentCardToken/{id}` | `operation--paymentCardToken--id--put` | Insert or update record. | `paymentCardToken` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--paymentCardToken-delete` | DELETE `/paymentCardToken` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--paymentCardToken-get` | GET `/paymentCardToken` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--paymentCardToken-patch` | PATCH `/paymentCardToken` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--paymentCardToken-post` | POST `/paymentCardToken` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--paymentCardToken-put` | PUT `/paymentCardToken` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--paymentCardToken--id--delete` | DELETE `/paymentCardToken/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--paymentCardToken--id--get` | GET `/paymentCardToken/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--paymentCardToken--id--patch` | PATCH `/paymentCardToken/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--paymentCardToken--id--put` | PUT `/paymentCardToken/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [paymentCardToken schemas](../schemas/paymentCardToken.md).

| Definition | Role |
| --- | --- |
| [`paymentCardToken`](../schemas/paymentCardToken.md#paymentcardtoken) | record body |
| [`paymentCardTokenCollection`](../schemas/paymentCardToken.md#paymentcardtokencollection) | collection page |
| [`paymentCardTokenSelectOptions`](../schemas/paymentCardToken.md#paymentcardtokenselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
