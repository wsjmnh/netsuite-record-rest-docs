# campaignTemplate

Browser tag `campaignTemplate` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/campaignTemplate`, instance `/campaignTemplate/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/campaignTemplate` | `operation--campaignTemplate-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/campaignTemplate` | `operation--campaignTemplate-get` | Get list of records. |  | 200 OK → `campaignTemplateCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/campaignTemplate` | `operation--campaignTemplate-patch` | Update records. | `campaignTemplateCollection` | 202 Accepted; default → `nsError` |
| POST | `/campaignTemplate` | `operation--campaignTemplate-post` | Insert record. | `campaignTemplate` | 200 OK → `campaignTemplate`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/campaignTemplate` | `operation--campaignTemplate-put` | Insert or update records. | `campaignTemplateCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/campaignTemplate/{id}` | `operation--campaignTemplate--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/campaignTemplate/{id}` | `operation--campaignTemplate--id--get` | Get record. |  | 200 OK → `campaignTemplate`; 202 Accepted; default → `nsError` |
| PATCH | `/campaignTemplate/{id}` | `operation--campaignTemplate--id--patch` | Update record. | `campaignTemplate` | 200 OK → `campaignTemplate`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/campaignTemplate/{id}` | `operation--campaignTemplate--id--put` | Insert or update record. | `campaignTemplate` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--campaignTemplate-delete` | DELETE `/campaignTemplate` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignTemplate-get` | GET `/campaignTemplate` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignTemplate-patch` | PATCH `/campaignTemplate` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignTemplate-post` | POST `/campaignTemplate` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--campaignTemplate-put` | PUT `/campaignTemplate` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignTemplate--id--delete` | DELETE `/campaignTemplate/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignTemplate--id--get` | GET `/campaignTemplate/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignTemplate--id--patch` | PATCH `/campaignTemplate/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--campaignTemplate--id--put` | PUT `/campaignTemplate/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [campaignTemplate schemas](../schemas/campaignTemplate.md).

| Definition | Role |
| --- | --- |
| [`campaignTemplate`](../schemas/campaignTemplate.md#campaigntemplate) | record body |
| [`campaignTemplateCollection`](../schemas/campaignTemplate.md#campaigntemplatecollection) | collection page |
| [`campaignTemplateSelectOptions`](../schemas/campaignTemplate.md#campaigntemplateselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
