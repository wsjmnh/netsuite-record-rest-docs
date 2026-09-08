# emailTemplate

Browser tag `emailTemplate` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/emailTemplate`, instance `/emailTemplate/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/emailTemplate` | `operation--emailTemplate-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/emailTemplate` | `operation--emailTemplate-get` | Get list of records. |  | 200 OK → `emailTemplateCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/emailTemplate` | `operation--emailTemplate-patch` | Update records. | `emailTemplateCollection` | 202 Accepted; default → `nsError` |
| POST | `/emailTemplate` | `operation--emailTemplate-post` | Insert record. | `emailTemplate` | 200 OK → `emailTemplate`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/emailTemplate` | `operation--emailTemplate-put` | Insert or update records. | `emailTemplateCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/emailTemplate/{id}` | `operation--emailTemplate--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/emailTemplate/{id}` | `operation--emailTemplate--id--get` | Get record. |  | 200 OK → `emailTemplate`; 202 Accepted; default → `nsError` |
| PATCH | `/emailTemplate/{id}` | `operation--emailTemplate--id--patch` | Update record. | `emailTemplate` | 200 OK → `emailTemplate`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/emailTemplate/{id}` | `operation--emailTemplate--id--put` | Insert or update record. | `emailTemplate` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--emailTemplate-delete` | DELETE `/emailTemplate` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--emailTemplate-get` | GET `/emailTemplate` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--emailTemplate-patch` | PATCH `/emailTemplate` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--emailTemplate-post` | POST `/emailTemplate` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--emailTemplate-put` | PUT `/emailTemplate` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--emailTemplate--id--delete` | DELETE `/emailTemplate/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--emailTemplate--id--get` | GET `/emailTemplate/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--emailTemplate--id--patch` | PATCH `/emailTemplate/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--emailTemplate--id--put` | PUT `/emailTemplate/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [emailTemplate schemas](../schemas/emailTemplate.md).

| Definition | Role |
| --- | --- |
| [`emailTemplate`](../schemas/emailTemplate.md#emailtemplate) | record body |
| [`emailTemplateCollection`](../schemas/emailTemplate.md#emailtemplatecollection) | collection page |
| [`emailTemplateSelectOptions`](../schemas/emailTemplate.md#emailtemplateselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.
