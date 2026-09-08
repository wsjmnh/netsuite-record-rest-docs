# paymentMethod

Browser tag `paymentMethod` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/paymentMethod`, instance `/paymentMethod/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/paymentMethod` | `operation--paymentMethod-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/paymentMethod` | `operation--paymentMethod-get` | Get list of records. |  | 200 OK → `paymentMethodCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/paymentMethod` | `operation--paymentMethod-patch` | Update records. | `paymentMethodCollection` | 202 Accepted; default → `nsError` |
| POST | `/paymentMethod` | `operation--paymentMethod-post` | Insert record. | `paymentMethod` | 200 OK → `paymentMethod`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/paymentMethod` | `operation--paymentMethod-put` | Insert or update records. | `paymentMethodCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/paymentMethod/{id}` | `operation--paymentMethod--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/paymentMethod/{id}` | `operation--paymentMethod--id--get` | Get record. |  | 200 OK → `paymentMethod`; 202 Accepted; default → `nsError` |
| PATCH | `/paymentMethod/{id}` | `operation--paymentMethod--id--patch` | Update record. | `paymentMethod` | 200 OK → `paymentMethod`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/paymentMethod/{id}` | `operation--paymentMethod--id--put` | Insert or update record. | `paymentMethod` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--paymentMethod-delete` | DELETE `/paymentMethod` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--paymentMethod-get` | GET `/paymentMethod` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--paymentMethod-patch` | PATCH `/paymentMethod` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--paymentMethod-post` | POST `/paymentMethod` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--paymentMethod-put` | PUT `/paymentMethod` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--paymentMethod--id--delete` | DELETE `/paymentMethod/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--paymentMethod--id--get` | GET `/paymentMethod/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--paymentMethod--id--patch` | PATCH `/paymentMethod/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--paymentMethod--id--put` | PUT `/paymentMethod/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [paymentMethod schemas](../schemas/paymentMethod.md).

| Definition | Role |
| --- | --- |
| [`paymentMethod`](../schemas/paymentMethod.md#paymentmethod) | record body |
| [`paymentMethod-visualsCollection`](../schemas/paymentMethod.md#paymentmethod-visualscollection) | sublist/collection |
| [`paymentMethod-visualsElement`](../schemas/paymentMethod.md#paymentmethod-visualselement) | sublist/element |
| [`paymentMethodCollection`](../schemas/paymentMethod.md#paymentmethodcollection) | collection page |
| [`paymentMethodSelectOptions`](../schemas/paymentMethod.md#paymentmethodselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `visuals` | [`paymentMethod-visualsCollection`](../schemas/paymentMethod.md#paymentmethod-visualscollection) | [`paymentMethod-visualsElement`](../schemas/paymentMethod.md#paymentmethod-visualselement) |
