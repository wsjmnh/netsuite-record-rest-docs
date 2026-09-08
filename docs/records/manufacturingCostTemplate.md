# manufacturingCostTemplate

Browser tag `manufacturingCostTemplate` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/manufacturingCostTemplate`, instance `/manufacturingCostTemplate/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/manufacturingCostTemplate` | `operation--manufacturingCostTemplate-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/manufacturingCostTemplate` | `operation--manufacturingCostTemplate-get` | Get list of records. |  | 200 OK → `manufacturingCostTemplateCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/manufacturingCostTemplate` | `operation--manufacturingCostTemplate-patch` | Update records. | `manufacturingCostTemplateCollection` | 202 Accepted; default → `nsError` |
| POST | `/manufacturingCostTemplate` | `operation--manufacturingCostTemplate-post` | Insert record. | `manufacturingCostTemplate` | 200 OK → `manufacturingCostTemplate`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/manufacturingCostTemplate` | `operation--manufacturingCostTemplate-put` | Insert or update records. | `manufacturingCostTemplateCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/manufacturingCostTemplate/{id}` | `operation--manufacturingCostTemplate--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/manufacturingCostTemplate/{id}` | `operation--manufacturingCostTemplate--id--get` | Get record. |  | 200 OK → `manufacturingCostTemplate`; 202 Accepted; default → `nsError` |
| PATCH | `/manufacturingCostTemplate/{id}` | `operation--manufacturingCostTemplate--id--patch` | Update record. | `manufacturingCostTemplate` | 200 OK → `manufacturingCostTemplate`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/manufacturingCostTemplate/{id}` | `operation--manufacturingCostTemplate--id--put` | Insert or update record. | `manufacturingCostTemplate` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--manufacturingCostTemplate-delete` | DELETE `/manufacturingCostTemplate` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--manufacturingCostTemplate-get` | GET `/manufacturingCostTemplate` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--manufacturingCostTemplate-patch` | PATCH `/manufacturingCostTemplate` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--manufacturingCostTemplate-post` | POST `/manufacturingCostTemplate` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--manufacturingCostTemplate-put` | PUT `/manufacturingCostTemplate` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--manufacturingCostTemplate--id--delete` | DELETE `/manufacturingCostTemplate/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--manufacturingCostTemplate--id--get` | GET `/manufacturingCostTemplate/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--manufacturingCostTemplate--id--patch` | PATCH `/manufacturingCostTemplate/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--manufacturingCostTemplate--id--put` | PUT `/manufacturingCostTemplate/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [manufacturingCostTemplate schemas](../schemas/manufacturingCostTemplate.md).

| Definition | Role |
| --- | --- |
| [`manufacturingCostTemplate`](../schemas/manufacturingCostTemplate.md#manufacturingcosttemplate) | record body |
| [`manufacturingCostTemplate-costDetailCollection`](../schemas/manufacturingCostTemplate.md#manufacturingcosttemplate-costdetailcollection) | sublist/collection |
| [`manufacturingCostTemplate-costDetailElement`](../schemas/manufacturingCostTemplate.md#manufacturingcosttemplate-costdetailelement) | sublist/element |
| [`manufacturingCostTemplateCollection`](../schemas/manufacturingCostTemplate.md#manufacturingcosttemplatecollection) | collection page |
| [`manufacturingCostTemplateSelectOptions`](../schemas/manufacturingCostTemplate.md#manufacturingcosttemplateselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `costDetail` | [`manufacturingCostTemplate-costDetailCollection`](../schemas/manufacturingCostTemplate.md#manufacturingcosttemplate-costdetailcollection) | [`manufacturingCostTemplate-costDetailElement`](../schemas/manufacturingCostTemplate.md#manufacturingcosttemplate-costdetailelement) |
