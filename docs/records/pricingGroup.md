# pricingGroup

Browser tag `pricingGroup` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/pricingGroup`, instance `/pricingGroup/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/pricingGroup` | `operation--pricingGroup-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/pricingGroup` | `operation--pricingGroup-get` | Get list of records. |  | 200 OK → `pricingGroupCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/pricingGroup` | `operation--pricingGroup-patch` | Update records. | `pricingGroupCollection` | 202 Accepted; default → `nsError` |
| POST | `/pricingGroup` | `operation--pricingGroup-post` | Insert record. | `pricingGroup` | 200 OK → `pricingGroup`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/pricingGroup` | `operation--pricingGroup-put` | Insert or update records. | `pricingGroupCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/pricingGroup/{id}` | `operation--pricingGroup--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/pricingGroup/{id}` | `operation--pricingGroup--id--get` | Get record. |  | 200 OK → `pricingGroup`; 202 Accepted; default → `nsError` |
| PATCH | `/pricingGroup/{id}` | `operation--pricingGroup--id--patch` | Update record. | `pricingGroup` | 200 OK → `pricingGroup`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/pricingGroup/{id}` | `operation--pricingGroup--id--put` | Insert or update record. | `pricingGroup` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--pricingGroup-delete` | DELETE `/pricingGroup` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--pricingGroup-get` | GET `/pricingGroup` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--pricingGroup-patch` | PATCH `/pricingGroup` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--pricingGroup-post` | POST `/pricingGroup` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--pricingGroup-put` | PUT `/pricingGroup` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--pricingGroup--id--delete` | DELETE `/pricingGroup/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--pricingGroup--id--get` | GET `/pricingGroup/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--pricingGroup--id--patch` | PATCH `/pricingGroup/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--pricingGroup--id--put` | PUT `/pricingGroup/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [pricingGroup schemas](../schemas/pricingGroup.md).

| Definition | Role |
| --- | --- |
| [`pricingGroup`](../schemas/pricingGroup.md#pricinggroup) | record body |
| [`pricingGroupCollection`](../schemas/pricingGroup.md#pricinggroupcollection) | collection page |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
