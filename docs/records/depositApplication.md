# depositApplication

Browser tag `depositApplication` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/depositApplication`, instance `/depositApplication/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/depositApplication` | `operation--depositApplication-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/depositApplication` | `operation--depositApplication-get` | Get list of records. |  | 200 OK → `depositApplicationCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/depositApplication` | `operation--depositApplication-patch` | Update records. | `depositApplicationCollection` | 202 Accepted; default → `nsError` |
| POST | `/depositApplication` | `operation--depositApplication-post` | Insert record. | `depositApplication` | 200 OK → `depositApplication`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/depositApplication` | `operation--depositApplication-put` | Insert or update records. | `depositApplicationCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/depositApplication/{id}` | `operation--depositApplication--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/depositApplication/{id}` | `operation--depositApplication--id--get` | Get record. |  | 200 OK → `depositApplication`; 202 Accepted; default → `nsError` |
| PATCH | `/depositApplication/{id}` | `operation--depositApplication--id--patch` | Update record. | `depositApplication` | 200 OK → `depositApplication`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/depositApplication/{id}` | `operation--depositApplication--id--put` | Insert or update record. | `depositApplication` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--depositApplication-delete` | DELETE `/depositApplication` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--depositApplication-get` | GET `/depositApplication` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--depositApplication-patch` | PATCH `/depositApplication` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--depositApplication-post` | POST `/depositApplication` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--depositApplication-put` | PUT `/depositApplication` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--depositApplication--id--delete` | DELETE `/depositApplication/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--depositApplication--id--get` | GET `/depositApplication/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--depositApplication--id--patch` | PATCH `/depositApplication/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--depositApplication--id--put` | PUT `/depositApplication/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [depositApplication schemas](../schemas/depositApplication.md).

| Definition | Role |
| --- | --- |
| [`depositApplication`](../schemas/depositApplication.md#depositapplication) | record body |
| [`depositApplication-accountingBookDetailCollection`](../schemas/depositApplication.md#depositapplication-accountingbookdetailcollection) | sublist/collection |
| [`depositApplication-accountingBookDetailElement`](../schemas/depositApplication.md#depositapplication-accountingbookdetailelement) | sublist/element |
| [`depositApplication-appliedRulesCollection`](../schemas/depositApplication.md#depositapplication-appliedrulescollection) | sublist/collection |
| [`depositApplication-appliedRulesElement`](../schemas/depositApplication.md#depositapplication-appliedruleselement) | sublist/element |
| [`depositApplication-applyCollection`](../schemas/depositApplication.md#depositapplication-applycollection) | sublist/collection |
| [`depositApplication-applyElement`](../schemas/depositApplication.md#depositapplication-applyelement) | sublist/element |
| [`depositApplicationCollection`](../schemas/depositApplication.md#depositapplicationcollection) | collection page |
| [`depositApplicationSelectOptions`](../schemas/depositApplication.md#depositapplicationselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`depositApplication-accountingBookDetailCollection`](../schemas/depositApplication.md#depositapplication-accountingbookdetailcollection) | [`depositApplication-accountingBookDetailElement`](../schemas/depositApplication.md#depositapplication-accountingbookdetailelement) |
| `appliedRules` | [`depositApplication-appliedRulesCollection`](../schemas/depositApplication.md#depositapplication-appliedrulescollection) | [`depositApplication-appliedRulesElement`](../schemas/depositApplication.md#depositapplication-appliedruleselement) |
| `apply` | [`depositApplication-applyCollection`](../schemas/depositApplication.md#depositapplication-applycollection) | [`depositApplication-applyElement`](../schemas/depositApplication.md#depositapplication-applyelement) |
