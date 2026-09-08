# pricePlan

Browser tag `pricePlan` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/pricePlan`, instance `/pricePlan/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/pricePlan` | `operation--pricePlan-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/pricePlan` | `operation--pricePlan-get` | Get list of records. |  | 200 OK → `pricePlanCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/pricePlan` | `operation--pricePlan-patch` | Update records. | `pricePlanCollection` | 202 Accepted; default → `nsError` |
| POST | `/pricePlan` | `operation--pricePlan-post` | Insert record. | `pricePlan` | 200 OK → `pricePlan`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/pricePlan` | `operation--pricePlan-put` | Insert or update records. | `pricePlanCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/pricePlan/{id}` | `operation--pricePlan--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/pricePlan/{id}` | `operation--pricePlan--id--get` | Get record. |  | 200 OK → `pricePlan`; 202 Accepted; default → `nsError` |
| PATCH | `/pricePlan/{id}` | `operation--pricePlan--id--patch` | Update record. | `pricePlan` | 200 OK → `pricePlan`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/pricePlan/{id}` | `operation--pricePlan--id--put` | Insert or update record. | `pricePlan` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--pricePlan-delete` | DELETE `/pricePlan` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--pricePlan-get` | GET `/pricePlan` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--pricePlan-patch` | PATCH `/pricePlan` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--pricePlan-post` | POST `/pricePlan` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--pricePlan-put` | PUT `/pricePlan` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--pricePlan--id--delete` | DELETE `/pricePlan/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--pricePlan--id--get` | GET `/pricePlan/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--pricePlan--id--patch` | PATCH `/pricePlan/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--pricePlan--id--put` | PUT `/pricePlan/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [pricePlan schemas](../schemas/pricePlan.md).

| Definition | Role |
| --- | --- |
| [`pricePlan`](../schemas/pricePlan.md#priceplan) | record body |
| [`pricePlan-priceTiersCollection`](../schemas/pricePlan.md#priceplan-pricetierscollection) | sublist/collection |
| [`pricePlan-priceTiersElement`](../schemas/pricePlan.md#priceplan-pricetierselement) | sublist/element |
| [`pricePlanCollection`](../schemas/pricePlan.md#priceplancollection) | collection page |
| [`pricePlanSelectOptions`](../schemas/pricePlan.md#priceplanselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `priceTiers` | [`pricePlan-priceTiersCollection`](../schemas/pricePlan.md#priceplan-pricetierscollection) | [`pricePlan-priceTiersElement`](../schemas/pricePlan.md#priceplan-pricetierselement) |
