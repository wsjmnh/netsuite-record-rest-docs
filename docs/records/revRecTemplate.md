# revRecTemplate

Browser tag `revRecTemplate` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/revRecTemplate`, instance `/revRecTemplate/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/revRecTemplate` | `operation--revRecTemplate-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/revRecTemplate` | `operation--revRecTemplate-get` | Get list of records. |  | 200 OK → `revRecTemplateCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/revRecTemplate` | `operation--revRecTemplate-patch` | Update records. | `revRecTemplateCollection` | 202 Accepted; default → `nsError` |
| POST | `/revRecTemplate` | `operation--revRecTemplate-post` | Insert record. | `revRecTemplate` | 200 OK → `revRecTemplate`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/revRecTemplate` | `operation--revRecTemplate-put` | Insert or update records. | `revRecTemplateCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/revRecTemplate/{id}` | `operation--revRecTemplate--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/revRecTemplate/{id}` | `operation--revRecTemplate--id--get` | Get record. |  | 200 OK → `revRecTemplate`; 202 Accepted; default → `nsError` |
| PATCH | `/revRecTemplate/{id}` | `operation--revRecTemplate--id--patch` | Update record. | `revRecTemplate` | 200 OK → `revRecTemplate`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/revRecTemplate/{id}` | `operation--revRecTemplate--id--put` | Insert or update record. | `revRecTemplate` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--revRecTemplate-delete` | DELETE `/revRecTemplate` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--revRecTemplate-get` | GET `/revRecTemplate` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--revRecTemplate-patch` | PATCH `/revRecTemplate` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--revRecTemplate-post` | POST `/revRecTemplate` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--revRecTemplate-put` | PUT `/revRecTemplate` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--revRecTemplate--id--delete` | DELETE `/revRecTemplate/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--revRecTemplate--id--get` | GET `/revRecTemplate/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--revRecTemplate--id--patch` | PATCH `/revRecTemplate/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--revRecTemplate--id--put` | PUT `/revRecTemplate/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [revRecTemplate schemas](../schemas/revRecTemplate.md).

| Definition | Role |
| --- | --- |
| [`revRecTemplate`](../schemas/revRecTemplate.md#revrectemplate) | record body |
| [`revRecTemplate-recurrenceCollection`](../schemas/revRecTemplate.md#revrectemplate-recurrencecollection) | sublist/collection |
| [`revRecTemplate-recurrenceElement`](../schemas/revRecTemplate.md#revrectemplate-recurrenceelement) | sublist/element |
| [`revRecTemplateCollection`](../schemas/revRecTemplate.md#revrectemplatecollection) | collection page |
| [`revRecTemplateSelectOptions`](../schemas/revRecTemplate.md#revrectemplateselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `recurrence` | [`revRecTemplate-recurrenceCollection`](../schemas/revRecTemplate.md#revrectemplate-recurrencecollection) | [`revRecTemplate-recurrenceElement`](../schemas/revRecTemplate.md#revrectemplate-recurrenceelement) |
