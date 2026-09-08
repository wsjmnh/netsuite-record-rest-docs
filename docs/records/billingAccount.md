# billingAccount

Browser tag `billingAccount` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/billingAccount`, instance `/billingAccount/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/billingAccount` | `operation--billingAccount-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/billingAccount` | `operation--billingAccount-get` | Get list of records. |  | 200 OK → `billingAccountCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/billingAccount` | `operation--billingAccount-patch` | Update records. | `billingAccountCollection` | 202 Accepted; default → `nsError` |
| POST | `/billingAccount` | `operation--billingAccount-post` | Insert record. | `billingAccount` | 200 OK → `billingAccount`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/billingAccount` | `operation--billingAccount-put` | Insert or update records. | `billingAccountCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/billingAccount/{id}` | `operation--billingAccount--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/billingAccount/{id}` | `operation--billingAccount--id--get` | Get record. |  | 200 OK → `billingAccount`; 202 Accepted; default → `nsError` |
| PATCH | `/billingAccount/{id}` | `operation--billingAccount--id--patch` | Update record. | `billingAccount` | 200 OK → `billingAccount`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/billingAccount/{id}` | `operation--billingAccount--id--put` | Insert or update record. | `billingAccount` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--billingAccount-delete` | DELETE `/billingAccount` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--billingAccount-get` | GET `/billingAccount` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--billingAccount-patch` | PATCH `/billingAccount` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--billingAccount-post` | POST `/billingAccount` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--billingAccount-put` | PUT `/billingAccount` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--billingAccount--id--delete` | DELETE `/billingAccount/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--billingAccount--id--get` | GET `/billingAccount/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--billingAccount--id--patch` | PATCH `/billingAccount/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--billingAccount--id--put` | PUT `/billingAccount/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [billingAccount schemas](../schemas/billingAccount.md).

| Definition | Role |
| --- | --- |
| [`billingAccount`](../schemas/billingAccount.md#billingaccount) | record body |
| [`billingAccountCollection`](../schemas/billingAccount.md#billingaccountcollection) | collection page |
| [`billingAccountSelectOptions`](../schemas/billingAccount.md#billingaccountselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
